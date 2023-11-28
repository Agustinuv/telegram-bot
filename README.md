# Telegram bot API

## Author: Agustín Urrutia Vega

## Description

Idea: create a bot that sends you a message to remember the birthday of your friends and where you can add new birthdays to the database.

## Start

- You must create a .env file in the root of the project, with the following environment variables:

```
PORT= {port}
DB_USER= {user}
DB_PASSWORD= {password}
DB_DATABASE= {database}
```

- Install dependencies with `npm install`
- Start the postgresql server: `sudo service postgresql start`
- Commands to create the database:

  - `npx sequelize-cli db:drop`
  - `npx sequelize-cli db:create`
  - `npx sequelize-cli db:migrate`
  - `npx sequelize-cli db:seed:all`

- Finally, start the server with `npm start dev`

## Bibliography

Schema built with the tutorials of [Capsula 3](https://cursos.canvas.uc.cl/courses/39221/files/5753437/download?download_frd=1)

## Ayudas personales

- To create a new migration: `npx sequelize-cli migration:generate --name {migration-name}`

- To open the postgresql console: `sudo -u postgres psql`
- `\c {database name}`
- `\d "Users"`
- `select * from "Users";`
