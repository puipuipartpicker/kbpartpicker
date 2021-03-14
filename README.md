# kbpartpicker

## Initialize and Update Submodules
```
git submodule init
git submodule update
```

## Prerequisites
- Docker is installed 
---
## Setup
### Setup backend Env Vars

Create a `.env` file in the root of the `/backend` directory with the following contents
```
DB_USERNAME=kbpp
DB_PASSWORD=password
DB_HOST=db
DB_NAME=kbpartpicker
DB_PORT=5432
```

### Setup frontend Env Vars
Create two env files: 
- `.env.development.local`
- `.env.production.local`

both with the following contents
```
REACT_APP_API_URL=http://localhost:5000
```
---

## Running docker containers
### On First Run & On Dependency Updates
```bash
docker-compose build
docker-compose up

# or
docker-compose up --build
```
### On Subsequent Runs
```
docker-compose up
```
