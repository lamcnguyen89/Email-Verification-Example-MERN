Source for Signup and Login: https://www.youtube.com/watch?v=HGgyd1bYWsE
Source for email verification: https://www.youtube.com/watch?v=T6rElSLldyc&t=215s

## Steps in Signup and Login Development

1. Create a Server folder and init npm in it. Install required packages
2. Create Index.js file or the entry point file.
3. Set up the server configuration in the index.js file
4. Create the db.js file which connects the application to the MongoDB server.
5. Go to MongodB, Create new project and create a new cluster.
6. White list your IP address in Mongo for that cluster.Input that info into the env file.
7. Create the User Model. It is the user.js file
8. Create the register route. It is the users.js file in the routes folder. WE create the post route for adding a new user in the signup.
9. Create the login route. It is the auth.js file.
10. Import Routes. In the index.js file bring in the routes.
11. Create the clientside react app. It is the entire client folder.
12. Enter the client and install axios and react-router-dom. The axios package is to call the API routes. And React-router-dom is assigning jobs for components.
13. In client/index.js. Set up browserrouter
14. Create Signup component in react. IN the component folder. There is the SingIp folder with an index.jsx file. Set up the front end code for it.
15. Create the login component for react. It is in the Components/Login folder in the client folder of the app.
16. Assign Routes. In App.js in client folder

## Steps in Verification Development

1. Create transporter to send email. This is the sendEmail.js file in the utils folder.
2. Create the environmental variables file. It is the .env file.
3. Create the user model. It is the user.js file. Add a boolean field called "verified"
4. Create the token model. It is the token.js file in the models folder. This token creates a mongoose model of the token that will be sent to the server and the server will send it to an email address.
5. Send verification link after signup. It is the user.js file in the routes filder.
6. Verify link sent by email in routes/user.js file. It is the router.get function.
7. Resend link if not verified.It is a route in the routes/auth.js file in the router.post function. Just adding some extra code to it.
8. Add a few changes to the signup page in componnents/signup/index.js
9. Create an email verified page in react. It is in components/EmailVerify/index.js

## Miscellaneous Notes

1. When setting up a mongodb address for the database. Create a new project, create a new cluster, and create a new user witha username and password. This new user with unique password will be input into the Mongodb address
2. JWT secret password. What is it? Let me find out.
3. **_To use a specific gmail account as a forwarding email to do email verification, go to your gmail account settings, enable 2FA and search for the option to add "App Passwords". App passwords allow you to create an password that is specific to whatever app or device you are trying to use which will prevent having to share your real GMAIL account password._**
4. You can use a different email service provider by modifying the SMTP settings in env file. Each email service provider has its own SMTP configuration, so refer to their documentation.
