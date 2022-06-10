## How to run locally
- Preparation
  - Rename .env.example to .env
  - Change .env properties if you need
  - Create postgresql database (by default mydb)
- Clone this repo
- `npm i` to install all required dependencies
- `npm run start:dev` to start local dev server (Default API: http://localhost:4000)

## Run with docker
You can also run this project with docker compose which contains nest.js app, postgresql db and pgadmin

`docker-compose up -d`

## Frontend
Source code of frontend application available in https://github.com/Uporold/cinemaddict-react

## Api routes
- [POST] `API/auth/register` register user by login, password, name and email
- [POST] `API/auth/login` login user by login and password
- [GET] `API/movies` get all movies
- [GET] `API/movies/:movieId` get movie by id
- [PATCH] `API/movies/:movieId/status` update user status of movie
- [GET] `API/comments/:movieId` get movie comments
- [POST] `API/comments/:movieId` create new comment
- [DELETE] `API/comments/:commentId` delete comment
