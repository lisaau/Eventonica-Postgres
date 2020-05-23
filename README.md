# Eventonica with Postgres

Eventonica is a web app to manage events from [Techtonica's curriculum](https://github.com/Techtonica/curriculum/tree/master/projects/eventonica). This repo includes part 6 listed in the [Overview](#overview).



## Overview

The project is split into seven phases covering various topics, some of which are in a different GitHub repo.

| Project Outline                                              | Project Repo                                                 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Part 1 - Object-Oriented Programming](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part1-objects.md) | [Eventonica](https://github.com/lisaau/Eventonica)           |
| [Part 2 - Testing](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part2-testing.md) | [Eventonica](https://github.com/lisaau/Eventonica)           |
| [Part 3 - jQuery UI](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part3-jquery-ui.md) | [Eventonica](https://github.com/lisaau/Eventonica)           |
| [Part 4 - API's](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part4-apis.md) | [Eventonica-API](https://github.com/lisaau/Eventonica-API)   |
| [Part 5 - Express Backend](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part5-express-backend.md) | [Eventonica-With-Express](https://github.com/lisaau/Eventonica-Express) |
| [Part 6 - Postgres Database](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part6-postgres.md) | [Eventonica-Postgres](https://github.com/lisaau/Eventonica-Postgres) |
| [Part 7 - React Frontend](https://github.com/Techtonica/curriculum/blob/master/projects/eventonica/eventonica-part7-react.md) | [Eventonica-React](https://github.com/lisaau/Eventonica-React) |



### Part 5

The project builds on part 1-5. In addition to an **object-oriented-programming** approach to set up the functionality, **jasmine** for unit testing, and **jQuery** for the UI, utilizing **Ticketmaster's API** to add additional events, adding an **Express server**, this part of the project focuses on the setting up a **Postgres database**.



## Running the app

1. Clone this directory/save files in this directory

2. Change into that directory and install dependencies:

   ```
   npm install
   ```

3. Set up the database using PostgreSQL. Make sure you have [PostgreSQL](https://wiki.postgresql.org/wiki/Homebrew) installed, which can be installed using [homebrew](https://brew.sh/). Take the eventonica.sql file and restore the database by running:

   ```
   CREATE DATABASE eventonica
   psql eventonica < eventonica.sql 
   ```

4. Run the Express server by running:

   ```bash
   node index.js
   ```

5. View the site on http://localhost:3000/

6. Running Mocha tests/Supertest - integration tests to test REST API's written in ExpressJS

   - Use `mocha` to run integration tests

   