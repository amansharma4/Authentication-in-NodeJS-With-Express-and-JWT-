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
