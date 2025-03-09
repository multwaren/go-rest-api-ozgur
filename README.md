## REST API OZGUR DOGAN GUNES


## Goals
The goal of this project is to develop a basic REST API using the Go programming
language and the Gin-Gonic framework. The API should be capable of interacting with a
database (e.g. PostgreSQL and SQLite). Additionally, the project should utilize
containerization to develop the application within a containerized environment

### Core Technologies

- **Programming Language**: The project is implemented using the Go programming language.
- **Framework**: The Gin-Gonic framework is utilized for building the REST API.


## Requirements

- Go 1.18 or higher recommended(1.23.0)
- Postgresql
- Docker

### Local Installation

1. Clone the repository:

```bash
git clone https://github.com/multwaren/go-rest-api-ozgur.git
cd go-rest-api-ozgur
```

 After cloning this repo to your local machine you should navigate to the directory.
 2. Create an .env file, credentials used in this app listed below
 nano .env 
```
PG_HOST=db
PG_PORT=5432
PG_USER=postgres
PG_NAME=bookclub
PG_PASSWORD=sifre

```

```
docker compose up 
```
Build the containers and it will ben run it.


## TEST
You can either use Insomnia or visit; 
```
http://localhost:8080/"WRITE-A-ROUTE-HERE"
```
You can try and use all the endpoints listed below:

You do not need to use the User system to access these endpoints. However, please note that all endpoints are publicly accessible, except for the `DELETE` method, which is a protected route and can only be accessed by Admin users.

```
- /api/v1/auth/register
- /api/v1/auth/login
- /api/v1/auth/refresh-token

- /api/v1/books
- /api/v1/book/"Book ID"
- /api/v1/authors
- /api/v1/author/"Author ID"
- /api/v1/reviews
- /api/v1/review/"Review ID"
```
## Swaagger DOCS
Can be accessed from http://localhost:8080/swagger/index.html