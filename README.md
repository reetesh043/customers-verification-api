# customers-verification-api

## Introduction
In this article, we will see how to easily create our own REST API server to be accessible on the internet without coding and without the need to host it on any hosting provider.
So let's get started.

## Setup local environment
Create a new folder with the name customers-verifications-api.

Navigate inside the folder from the command line and execute the following command
```
npm init -y
```
This will create a package.json file inside your project.

## Install the json-server npm package by executing the following command
```
npm install json-server
```
Create a new file with the name .gitignore with the entry for node_modules inside it so the node_modules folder will not be pushed to GitHub while pushing the code to the GitHub repository.

Create a new file with the name db.json and add the following contents inside it:
```
{
  "customers": [
    {
      "id": 1,
      "name": "Reetesh",
      "age": 30,
      "email": "reet.k@test.com"
    },
    {
      "name": "Kumar",
      "id": 2,
      "age": 40,
      "email": "kumr.k@test.com"
    }
  ]
}
```
Open package.json file and add the scripts section inside it:
```
"scripts": {
  "start": "json-server db.json"
}
```
Now, start the application by running the npm start command from the terminal.

