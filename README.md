<div align="center" style="padding-top: 10px;">
<img src="https://cdn-images-1.medium.com/max/1000/1*IvCDlfi3vQfgyKO1eFv4jA.png" alt="graphql logo" width="30%">
<img src="./images/postgresql.png" alt="postgres logo" width="30%" >
<img src="./images/knex.png" alt="knex logo" width="30%" >
</div>

# cc9-michelin-restaurant-api

This was created during my time as a student at Code Chrysalis.

## 1. Set Up

Run `yarn` to install dependencies.

You will need the [PostgresApp](https://postgresapp.com/) installed. Run `psql` and create a database name michelin by running `create database michelin;`. Connect to your database by running `\c michelin`.

Run `yarn migrate` to set up the database.

Run the following commands to seed the database. Some tables are dependent on others, so it's important that you run them in this order:

`yarn seed --specific=cuisines_seeds.js`

`yarn seed --specific=countries_seeds.js`

`yarn seed --specific=cities_seeds.js`

`yarn seed --specific=restaurants_seeds.js`

## 2. Server Quick Start

Run `yarn start` to start the server.

Run `yarn dev` instead to automatically restart the server when any file changes thanks to `nodemon`.

Visit `http://localhost:3000` to test that the server is running.

Visit `http://localhost:3000/graphql` to see documentation and fulfill GraphQL queries.
