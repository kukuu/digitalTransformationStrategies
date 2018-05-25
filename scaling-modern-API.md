Scaling APIs & Separation of Conerns - NodeJS

..............................................


Many modern applications separate the backend services from the frontend user interface. In this type of architecture, the backend will expose a web based API that the frontend client consumes. 

Typically, the backend will handle incoming requests and return a JSON or XML encoded response. The frontend will then be in charge of formatting, styling, and displaying this response to the user. We’ve all heard the term “separation of concerns” and applying it at this scale has many benefits.

The backend services can grow and evolve independent of the frontend client. New APIs, if properly versioned, can provide new features and functionality without breaking existing integrations. A single backend can interface with multiple clients and the frontend clients will not be limited to any specific framework or programming language. This means that your single backend can work with your app for both a web based implementation, your mobile app, and even with IoT devices.


Dependencies:
Run npm install express express-jwt auth0-api-jwt-rsa-validation --save to install the dependencies we are going to need.

1. The express dependency will pull down the express framework.

2. express-jwt library will give us functions to work with JSON Web Tokens.

3. auth0-api-jwt-rsa-validation will provide a helper function for getting our secret key.


Protecting API

...................

When you build your API initially it is unprotected and anyone can have access to it and call it.

 Let’s fix this by securing our endpoints with Auth0. Auth0 makes user identity . If you don’t already have an Auth0 account, signup for a free account here. Once you’ve signed up, navigate to your Auth0 dashboard and click on the New Client button to create a new Auth0 application.