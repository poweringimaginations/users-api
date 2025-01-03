# users-api
Implemented an API with PostgreSQL. The API manages user data and was deployed on Render. 

# steps
Created local PostgreSQL database (users_db)

Created a users table:
id (Primary Key, SERIAL)
first_name (VARCHAR)
last_name (VARCHAR)
email (VARCHAR, UNIQUE)

Turned this database into Render's PostgreSQL service. Using the external connection string I put the same data into the deployed database.

stored all database credentials in a .env file. /users endpoint now allows me to fetch data from the user database. The live API communicates with Render's PostgreSQL to database using the environment variables.

API: https://users-api-1rkb.onrender.com/users

used Postman to send GET requests to the /users endpoint to check that everything was running

TLDR;
local development -> deployed environment (Render)




