# CSL7510: Virtualization and Cloud Computing - Assessment 1

## Steps followed:
1. Created a basic CRUD web application in Golang using the `net/http` module and gorm as the ORM, along with a PostgreSQL database.
2. Created a Dockerfile called `Dockerfile.web` for building and running the web application. This Dockerfile uses a multi-stage build to build the application and then run it.
3. Created a Dockerfile called `Dockerfile.db` for installing and running the PostgreSQL database on a `Debian` base image, with the database data stored in a volume. The username and password for the database are `b20bb005` and `toor`, respectively.
4. A docker-compose.yml file was created to run both the web application and the database together. The web application is exposed on port 8080, and the database is exposed on port 5432.
5. The web application was tested using `curl` and `Postman` to ensure that it works as expected.

## Application endpoints:
1. `GET /users` - Returns a list of all the users in the database.
2. `POST /users` - Creates a new user in the database. The request body should contain a JSON object with the following fields: `name`, `email`.
3. `PUT /users` - Updates the user with the specified ID. The request body should contain a JSON object with the following fields: `id`, `name`, `email`.
4. `DELETE /users` - Deletes the user with the specified ID. The request body should contain a JSON object with the following fields: `id`.

## Author:
Name: Saahil Bhavsar
   
Roll No.: B20BB005
