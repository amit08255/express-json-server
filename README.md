# Mock API Server

This is simple mock API server built with json-server and expressjs.

# Getting Started

* Fork this repo

* Run `npm install` to install project dependencies.

* Run `npm start` to start expressjs server.

# Routes

Routes created come under namespace - /api

# Database for mock API

`db.json` file is used for mock API server. Data stored here is used to create APIs and routes.

# Routes

* `/api/users` - List all users in `db.json`
* `api/users/1` - List all users in `db/json` with ID - **1**