# Drupal development teamwork demo

## Setup the local development
- Make sure the local machine have **Lando** and **Docker Destop**
- Clone the project: `git clone https://github.com/alextrandev/hbc_drupal_workshop.git`
- Change working directory: `cd hbc_drupal_workshop`
- Install drupal core, vendor folder and nessesary files: `lando composer install`
- Import drupal configuratio: `lando drush cim`
- Optional: Ask for the db sql file and import with: `lando db-import NAME.sql`
- Start the project: `lando start`
- The terminal should giving the root url after finnish starting up

### To login as admin: 
- Run: `lando drush uli`
- Copy the link returned on the terminal
- Replace the base url `http://default/` with your own base url
- Paste it in a browser and you should be able to logged in and change admin password
