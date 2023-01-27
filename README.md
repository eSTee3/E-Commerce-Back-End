# E-commerce Back End Starter Code

# Installation
1. Download or clone this repo to your local machine
2. Create a `.env` file in the root of the directory (within your IDE of choice)
 - Copy/paste the following code into the .env file you created, changing the password to be your MySQL root password:
 ```
  DB_NAME = 'ecommerce_db'
  DB_USER = 'root'
  DB_PW = 'password'
 ```
3. Update the `'rootPassword'` within that file, to be your MySQL root password
4. Launch a terminal from the root of the same folder
5. Log into MySQL by entering `mysql -u root -p`, followed by entering your password
6. Enter `source db/schema.sql` to source the Database to your MySQL instance
7. Enter `use ecommerce_db`to change the in-use Database to "ecommerce_db"
8. Enter `exit` to go back to the standard terminal prompt
9. Enter `npm install` to install all required packages and wait for them to complete
10. Enter `npm run seed` to seed the newly created ecommerce_db Database
11. Enter `npm start` to initialize and launch the api server and complete this process

## User Story
**AS A** manager at an internet retail company...  **I WANT** a back end for my e-commerce website that uses the latest technologies...  **SO THAT** my company can compete with other e-commerce companies

## Acceptance Criteria
```
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```
