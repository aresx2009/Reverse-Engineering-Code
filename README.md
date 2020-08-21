# Reverse-Engineering-Code
Config folder:
middleware->isAuthenticated.js: Restricting routes a user is not allowed to visit if not logged in.
Config.json: connection config to server. Development, test or production.
passport.js:Telling passport we want to use a Local Strategy. We want login with a username/email and password.
 
Models folder:
Index.js: Import user’s data and connect to database.
User.js: Requiring bcrypt for password hashing. Using the bcryptjs version as the regular bcrypt module sometimes causes errors on Windows machines.
 
Public folder:
JS>login.js: javascript logic validate user entered username and password.
Members.js: javascript logic for members page.
Signup.js:  javascript logic Does a post to the signup route. If successful,redirect user to the members page.
Stylesheet: CSS stylesheet.
Login,members,signup.html: HTML files for each page.
 
Routes folder:
Api-routes.js: Login,logout and sign up route.Route for getting some data about our user to be used client side
html-routes.js:Checking if a user is logged in and redirecting the user to the correct page.
 
Package.json: NPM information.
Server.js: set up PORT, syncs database.