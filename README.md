# Mock API Server

This is simple mock API server built with json-server and expressjs.

# Getting Started

* Fork this repo

* Run `npm install` to install project dependencies.

* Run `npm start` to start expressjs server.

# Routes

Routes created come under namespace - /api

**A POST, PUT or PATCH request should include a Content-Type: application/json header to use the JSON in the request body. Otherwise it will result in a 200 OK but without changes being made to the data.**

# Database for mock API

`db.json` file is used for mock API server. Data stored here is used to create APIs and routes.

# Routes

* `/api/db` - Get entire database
* `/api/users` - List all users in `db.json`
* `api/users/1` - List all users in `db/json` with ID - **1**

# Adding Data

`POST` request to `/api/users` with `JSON` request allows you to add data to database.
Sample `JSON` request for adding data - `{"name": "Amit", "userId": 101}`

# Replacing Data

`PUT` request to `/api/users/1` with `JSON` request will replace data of user with ID **1** in database.

# Updating Data

`PATCH` request to `/api/users/1` with `JSON` request will replace data of user with ID **1** in database.

# Filter

Use . to access deep properties

`GET /posts?title=json-server&author=typicode`
`GET /posts?id=1&id=2`
`GET /comments?author.name=typicode`

#Paginate

Use `_page` and optionally `_limit` to paginate returned data.
In the Link header you'll get first, prev, next and last links.
`GET /posts?_page=7`
`GET /posts?_page=7&_limit=20`