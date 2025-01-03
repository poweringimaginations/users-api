# users-api
Implemented an API with PostgreSQL. The API manages user data and was deployed on Render. 

# steps
Created local PostgreSQL database (users_db)

Created a users table:
id (Primary Key, SERIAL)
first_name (VARCHAR)
last_name (VARCHAR)
email (VARCHAR, UNIQUE)

Transitioned this database into Render's PostgreSQL service. Using the external connection string I put the same data into the deployed database.

stored all database credentials in a .env file. /users endpoint now allows me to fetch data from the user database. The live API communicates with Render's PostgreSQL to database using the environment variables.

API: https://users-api-1rkb.onrender.com/users

used Postman to send GET requests to the /users endpoint to check that everything was running

# takeaways
- the backend manages data and communicates with the frontend to make everyhting work together
- information is stored in a database. here I created a users table in PostgreSQL which keeps track of user information such as names and email
- all this data can be accessed through an API using the /users endpoint
- for anyone to use the API, it needs to be live on the internet. Render PostgreSQL database and web services allowed me to deploy this
- keep sensitive information in .env files

TLDR;
local development -> deployed environment (Render)



