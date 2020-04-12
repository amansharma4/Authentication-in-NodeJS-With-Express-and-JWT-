# Authentication-in-NodeJS-With-Express-and-JWT-
###  Packages Required


You will be needing these following 'npm' packages. 

1. **express**
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications


2. **express-validator**
To Validate the body data on the server in the express framework, we will be using this library. It's a server-side data validation library. So, even if a malicious user bypasses the client-side verification, the server-side data validation will catch it and throw an error. 

3. **body-parser**
It is `nodejs` middleware for parsing the body data. 


4. **bcryptjs**
This library will be used to hash the password and then store it to database.This way even app administrators can't access the account of a user. 

5. **jsonwebtoken**
**jsonwebtoken** will be used to encrypt our data payload on registration and return a token. We can use that **token** to authenticate ourselves to secured pages like the dashboard. There would also an option to set the validity of those token, so you can specify how much time that token will last. 

6. **mongoose**
Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment. Mongoose supports both promises and callbacks.
###  Initiate Project

We will start by creating a node project. So, Create a new folder with the name 'node-auth' and follow the steps below. All the project files should be inside the 'node-auth' folder. 


```
npm init

```

***npm init*** will ask you some basic information about project. Now, you have created the node project, it's time to install the required packages. So, go ahead and install the packages by running the below command.

```javascript
npm install express express-validator body-parser bcryptjs jsonwebtoken mongoose --save
```

Now, create a file ***index.js*** and add this code. 

```javascript
// File : index.js

const express = require("express");
const bodyParser = require("body-parser");

const app = express();

// PORT
const PORT = process.env.PORT || 4000;

app.get("/", (req, res) => {
  res.json({ message: "API Working" });
});


app.listen(PORT, (req, res) => {
  console.log(`Server Started at PORT ${PORT}`);
});

```

If you type `node index.js` in the terminal, the server will start at PORT 4000. 

> You have successfully set up your NodeJS app application. It's time to set up the database to add more functionality. 

----
