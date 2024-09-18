0x05. NodeJS Basics 
............................................................................... 


0. Executing basic javascript with Node JS 
In the file 0-console.js, create a function named displayMessage that prints in STDOUT the string argument. 


1. Using Process stdin 
Create a program named 1-stdin.js that will be executed through command line:

It should display the message Welcome to Holberton School, what is your name? (followed by a new line)
The user should be able to input their name on a new line
The program should display Your name is: INPUT
When the user ends the program, it should display This important software is now closing (followed by a new line) 


2. Reading a file synchronously with Node JS 
Using the database database.csv (provided in project description), create a function countStudents in the file 2-read_file.js

Create a function named countStudents. It should accept a path in argument
The script should attempt to read the database file synchronously
If the database is not available, it should throw an error with the text Cannot load the database
If the database is available, it should log the following message to the console Number of students: NUMBER_OF_STUDENTS
It should log the number of students in each field, and the list with the following format: Number of students in FIELD: 6. List: LIST_OF_FIRSTNAMES
CSV file can contain empty lines (at the end) - and they are not a valid student! 


3. Reading a file asynchronously with Node JS 
Using the database database.csv (provided in project description), create a function countStudents in the file 3-read_file_async.js

Create a function named countStudents. It should accept a path in argument (same as in 2-read_file.js)
The script should attempt to read the database file asynchronously
The function should return a Promise
If the database is not available, it should throw an error with the text Cannot load the database
If the database is available, it should log the following message to the console Number of students: NUMBER_OF_STUDENTS
It should log the number of students in each field, and the list with the following format: Number of students in FIELD: 6. List: LIST_OF_FIRSTNAMES
CSV file can contain empty lines (at the end) - and they are not a valid student!


4. Create a small HTTP server using Node's HTTP module 
In a file named 4-http.js, create a small HTTP server using the http module:

It should be assigned to the variable app and this one must be exported
HTTP server should listen on port 1245
Displays Hello Holberton School! in the page body for any endpoint as plain text 


5. Create a more complex HTTP server using Node's HTTP module 
In a file named 5-http.js, create a small HTTP server using the http module:

It should be assigned to the variable app and this one must be exported
HTTP server should listen on port 1245
It should return plain text
When the URL path is /, it should display Hello Holberton School! in the page body
When the URL path is /students, it should display This is the list of our students followed by the same content as the file 3-read_file_async.js (with and without the database) - the name of the database must be passed as argument of the file
CSV file can contain empty lines (at the end) - and they are not a valid student! 


6. Create a small HTTP server using Express 
Install Express and in a file named 6-http_express.js, create a small HTTP server using Express module:

It should be assigned to the variable app and this one must be exported
HTTP server should listen on port 1245
Displays Hello Holberton School! in the page body for the endpoint / 


7. Create a more complex HTTP server using Express 
In a file named 7-http_express.js, recreate the small HTTP server using Express:

It should be assigned to the variable app and this one must be exported
HTTP server should listen on port 1245
It should return plain text
When the URL path is /, it should display Hello Holberton School! in the page body
When the URL path is /students, it should display This is the list of our students followed by the same content as the file 3-read_file_async.js (with and without the database) - the name of the database must be passed as argument of the file
CSV file can contain empty lines (at the end) - and they are not a valid student! 


8. Organize a complex HTTP server using Express 
Obviously writing every part of a server within a single file is not sustainable. Let’s create a full server in a directory named full_server.

Since you have used ES6 and Babel in the past projects, let’s use babel-node to allow to use ES6 functions like import or export. 
