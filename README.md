# User authentication server

NodeJs authentication server with Express framework.Only authorized users have access to database,in order to see infos there.

MongoDb and Mongoose used for storing info and user data (ID,email and hashed password).

Two login options:email and password or google OAuth2.0 authentication with passport.js package.

Checks if googleid exists or not in our database and saves it in our db.If user is authenticated he gain access to infos.

For more safety user's password are hashed and salted.Md5 and bcrypt packages used as cryptographic hash functions.

We send cookie to our browser to inform that this user is authenticate.Cookie expires when browser closes,unless that happens he can leave and come again with no verification.

