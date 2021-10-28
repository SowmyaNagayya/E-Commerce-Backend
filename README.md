# Homework 13: E-Commerce-Backend

## License
  The Project is licensed under the MIT License
  MIT License
  Copyright (c) 2021 SowmyaNagayya

  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
  
  The above copyright notice and this permission notice shall be included in all
  copies or substantial portions of the Software.
  
  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.;
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

  ## objectives
  E-Commerce Backend is a backend API (surprise surprise) that makes use of CRUD operations for a general eCommerce website. The API is built with Express.js and Sequelize to interact with a MySQL database. There are endpoints for categories, tags, and products. Products belong to a single category but can have multiple tags, and tags can be attributed to multiple products.


  ## Table of Contents 
  - [Installation instructions](#installationinstructions)
  - [Usage](#usage)
  - [License](#license)
  - [question](#Questions)
  
  ## Installation instructions
  First, download or clone the repository to your local machine. Then, from within the root directory, run:

  npm i
  to install all the necessary dependencies.

  Next, you will need to connect the application to a MySQL database running locally on your machine. First, make sure you have a MySQL server installed and running on your machine. After confirming you have a server runnning, you will need to create a .env file in the root directory to hold your database credentials. You will need to add the following three properties:

  DB_USER=<username>
  DB_PW=<password>
  DB_NAME='ecommerce_db'
  Once this is complete, you will need to instantiate the database via the provided schema.sql file. From your root directory, run:

  mysql -u <username> -p
  
  and enter your username and password credentials. Then, from inside your MySQL shell, run:

  source db/schema.sql // creates the database, or recreates if it already exists.
  quit
  Optionally, you may seed the database with provided dummy data contained in the /seeds directory by running:

  npm run seed
  
  from your root directory.

  The application should now be ready for use.

  ## Usage Instructions

  From the root directory, after confirming you've installed all prerequisites and set up the application, run:

  npm start
  The server will become live and will listen on the default port of 3001. Users can then make requests to three different endpoints:

  Categories:

  GET /api/categories/
  GET /api/categories/:categoryID
  POST /api/categories/
  PUT /api/categories/:categoryID
  DELETE /api/categories/:categoryID

  Tags:

  GET /api/tags/
  GET /api/tags/:tagID
  POST /api/tags/
  PUT /api/tags/:tagID
  DELETE /api/tags/:tagID
  
  Products:

  GET /api/products/
  GET /api/products/:productID
  POST /api/products/
  PUT /api/products/:productID
  DELETE /api/products/:productID

  ## Link to Demo
  https://drive.google.com/file/d/1aM6uljIaRH7ePFHG7JsVbq8wN10_lu1N/view?usp=sharing


  ## Questions
  Please email any questions to kkd.sowmya@gmail.com or reference my [GitHub profile](https://github.com/SowmyaNagayya).