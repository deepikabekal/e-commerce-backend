# e-commerce-backend

## Description
Back end for an e-commerce site with working Express.js API that uses Sequelize to interact with a MySQL database.

## Table of Contents
* [Installation](#installation)
* [Usage](#usage)
* [Preview](#preview)
* [Techologies Used](#technologiesused)
* [User Story](#userstory)
* [Acceptance Criteria](#acceptancecriteria)
* [Contributing](#contributing)
* [Questions](#questions)

## Installation
1. Make sure to have MySQL, Insomnia or Postman installed.
2. Clone this repo using ssh on your local machine.
```
git clone 
```
3. Open terminal and make sure to cd to the root of the repo.
4. Open the repo in your text editor.
5. Create a .env file at the root of the repo.
6. Copy and paste the following code in the .env file. Replace the value of DB_USER and DB_PW with your own credentials inside the quotes.
```
DB_USER = 'enter your MySQL username here.'
DB_PW = 'enter your MySQL password here.'
DB_NAME = 'ecommerce_db'
```
7. Install all the dependencies.
```
npm install
```
8. Open MySQL shell using the below command in the terminal and enter your password when prompted.
```
mysql -u root -p
```
9. Run the below commands to create and use the database.
```
source db/schema.sql
USE ecommerce_db;
```
10. Exit the MySQL shell by running the below command.
```
exit
```
11. In the terminal run the below command to seed the tables. 
```
npm run seed
```
12. Run the server using the below command.
```
node server.js
```

## Usage
1. Open Insomnia or Postman
2. Test the various endpoints at http://localhost:3001/

## Preview


##Technologies
ExpressJS
MySQL2
Sequelize


## User Story
```
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

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

## Contributing
1. Fork the repo.
2. Add feature or make changes.
3. Make a pull request for review.


