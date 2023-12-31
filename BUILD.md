# How to build the project

To use the application you need to go through several steps :

## 1 - Clone the repository in your IDE

Use git clone <repository URL> in your IDE to get the files.


## 2 - Install the packages 

Since the project is in two parts, front and back, we need to install the packages for each. 

From the root of the project, go into the frontend-angular directory and use npm install like this : 

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/45471758-67f2-4e12-8005-ecee0976a015)

It's the same thing for the backend, go into the backend-node directory and use npm install.

Now you may have all the necessary modules and packages.

## 3 - Create the user, the database, the tables and insert the values



You have to use PostgreSQL and create a user named "learningDbUser" with the password "learningDbUser" (Or you can put another and modify the sequelize config, I will show you this step)  and give him the database administrator role:

**CREATE USER "learningDbUser" WITH PASSWORD 'learningDbUser';**
**ALTER USER "learningDbUser" WITH SUPERUSER;**

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/844b467f-b2b4-4834-8bcf-f03d7b3c4c53)


Then create a database "LearningFactDb" with "learningDbUser" as the owner:

**CREATE DATABASE "LearningFactDb" OWNER "learningDbUser";**


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/29b0ea7c-291e-44aa-a350-6caf4b3434b8)


**I put a file named "CREATION TABLES AND INSERT VALUES.txt" in the root of the project.**

You can now open the SQL query tool in the "LearningFactDB" and run the script:

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/b9f2f0e8-5f79-4c4a-a6ad-d03229f1f463)

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/746cf58b-1d8a-45dc-8416-8a3cfcbd7352)



It should look like this : 

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/610df8dc-ab4e-4133-9fc6-06a70febfa63)


## 4 - Modify Sequelize config if needed

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/1abd897a-d937-40eb-84bd-b390fbee746e)

Here is the sequelize config, if you have a different password then change it there, the file is in ./backend-nodejs/sequelize.ts ( Don't forget to compile the typescript).


## 5 - Run the Node server

Go in the ./backend-nodejs directory and use "node app.js"

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/99103fe2-264d-4223-af4a-73a8857537c6)


## 6 - Run the Angular server 
Go in the ./frontend-angular directory and use "ng serve".

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/e33d2cfb-3735-4ef6-9903-029a0a4d52d3)


## 7 - Access the application

To access the home page just use this link **"http://localhost:4200/#/"**



![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/be8fa98e-fc65-42fa-ab5f-2d23f8976f42)


