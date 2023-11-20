# Customers-Verification-Api

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
Open the package.json file and add the scripts section inside it:

```
"scripts": {
  "start": "json-server db.json"
}
```

## Start the application
Now, start the application by running the npm start command from the terminal.
You will see the following screen when you access it at http://localhost:3000/

![Alt text](https://github.com/reetesh043/customers-verification-api/blob/main/json_server_1.png?raw=true)

If you click the /customers link under the resources section, you will see the following screen

![Alt text](https://github.com/reetesh043/customers-verification-api/blob/main/customer_resource.png?raw=true)

Congratulations! You've just written your own REST API server without writing a single line of code. Now we can make GET, POST, PUT, PATCH, and DELETE API calls to our own API.

## Deploy the application
Deploying the application that uses json-server is very easy.
You just have to create a GitHub repository push your local changes to that repository and access it with a specific URL from the browser.

Once the changes are pushed to the repository you can access your json-server by navigating to 
```
https://my-json-server.typicode.com/your_github_username/your_repository_name
```
for example https://my-json-server.typicode.com/reetesh043/customers-verification-api/customers

To learn more about json-server click [https://my-json-server.typicode.com/]



