# Base - Backend Express (Node)
Base Project for generating Backend APIs using Nodejs and Express for HTTP Server and MongoDB for database management.

## Features
This version of the base project supports the following features:
- HTTP server middleware management
- CORS Validation
- Error Handling
- Constants Management
- Basic Database Handling

## Requirements
In order to run the project, the following software is needed:
- [NVM for Windows](https://github.com/coreybutler/nvm-windows) - Node version manager, _recommended if you run projects with different Node versions (If you don't want NVM, just install latest [Node.js](https://nodejs.org/en/download/) version)_
- [MongoDB](https://www.mongodb.com/try/download/community) - Database Manager
- Yarn - Package manager, install with `npm install -g corepack`

The next ones are not required, but recommended
- [MongoDB Compass](https://www.mongodb.com/try/download/compass) - For DB management
- Nodemon - For debugging, install with `npm install -g nodemon`

## Setup & Run
In order to run the project follow the next steps, taking into account they are designed to run the project *locally*. URL's should change otherwise:
1. Clone repository
2. Create DB in MongoDB by name `nodejs-express` and collection name `users`
3. Create `.env` file in root folder of project, following `.env-example` structure with the following variables:
    - PORT=3000 - *(Or whatever is best)*
    - CORS_ORIGIN_WHITELIST=["localhost"] - *(This list allows hosts to connect)*
    - DATABASE_URL=mongodb://localhost:27017/nodejs-express - *(This is assuming you created DB with name nodejs-express)*
4. Run `yarn` to install all dependencies
5. Run `yarn start` for starting server or `yarn test` for starting server with `nodemon`


