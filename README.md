# E-Commerce Back End

## Description
This is the backend code for an E-commerce website. There is no front end for this code. The models and routes can be tested with Insomnia Core. A link to the walkthrough video can be found [here](https://www.youtube.com/watch?v=gtusl2h8TsU).
    
    
## Table of Contents:
* [Installation](#installation)
* [Usage](#usage)
* [Screenshots](#screenshots)
* [Questions](#questions)

## Installation
<pre>
git clone git@github.com:lwrnce/e-commerce.git
</pre>
then run the following command to install the required dependencies:
<pre>
npm install
</pre>

## Usage
To run the application, you have to first create and populate the database. In a terminal run the command
<pre>
mysql -u root -p
</pre>
And enter your password when prompted. Run the code from schema.sql:
<pre>
DROP DATABASE IF EXISTS ecommerce_db;

CREATE DATABASE ecommerce_db;
</pre>
You can not exit mysql.

Next create a .env file in the root directory. Enter your user name and password. It should look like the following:
<pre>
DB_NAME='ecommerce_db'
DB_USER='YourUsername'
DB_PW='YourPassword'
</pre>
Now you must populate the database by running the following command:
<pre>
node seeds/index.js
</pre>
Once that is complete you can start the server with:
<pre>
npm start
</pre>
You can now use the GET, POST, PUT, and DELETE routes via an application like Insomnia Core.

## Screenshots
![image](https://user-images.githubusercontent.com/64458077/121832238-7b35c880-cc7e-11eb-92d9-e90cd4a7814a.png)
![image](https://user-images.githubusercontent.com/64458077/121832245-7f61e600-cc7e-11eb-81cc-c1c58e871d3e.png)
![image](https://user-images.githubusercontent.com/64458077/121832262-8852b780-cc7e-11eb-8219-e7183c88342a.png)
![image](https://user-images.githubusercontent.com/64458077/121832273-8d176b80-cc7e-11eb-8896-676d47058699.png)






## Questions
If you have any questions, please contact me on [GitHub](https://github.com/lwrnce) or email me at lawrencyuen@gmail.com.
