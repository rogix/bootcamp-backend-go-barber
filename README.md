# GoBarber

This is a simple CRUD project that add some project and tasks to the project. It can Create, Delete, Update and Read projects.


## Built With

* [ExpressJS](https://expressjs.com/): is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
* [Nodemon](https://github.com/remy/nodemon#nodemon): is a tool that helps develop node.js based applications by automatically restarting the node application when file changes in the directory are detected.
* [Sucrase](https://github.com/alangpierce/sucrase): is an alternative to Babel that allows super-fast development builds.
* [docker](https://www.docker.com/): Docker is a set of platform as a service products that uses OS-level virtualization to deliver software in packages called containers.
* [postgres](https://docs.docker.com/engine/examples/postgresql_service/):The postgres database is a default database meant for use by users, utilities and third
party applications.
* [eslint](https://eslint.org/): a pluggable and configurable linter tool for identifying and reporting on patterns in JavaScript. Maintain your code quality with ease.
* [prettier](https://prettier.io/): an opinionated code formatter
* [sequelize](https://sequelize.org/): is a promise-based Node.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server.
* [bcryptjs](https://github.com/dcodeIO/bcrypt.js): optimized bcrypt in JavaScript with zero dependencies.

## Installation

*To install the necessary packages go to the root directory and run the following command:*

```
yarn install
```

*To run the app:*

```
yarn dev
```

## Docker

*To see which container is running:*

```
docker ps
```

*To see a list of all containers:*

```
docker ps -a
```

*To stop docker:*

```
docker stop database
```

*To run docker again:*

```
docker start database
```

*To visualize errors:*

```
docker log database
```

## Sequelize

We can use sequelize-cli to create our migrations.

*To create a table called ```users``` we can use the following command:*

```
yarn sequelize migration:create --name=create-users
```

After this a file will be automatically created inside the migrations folder.

*To run the migration:*

```
yarn sequelize db:migrate
```

This will created a table inside the database

*To undo the last migration:*

```
yarn sequelize db:migrate:undo
```

*To undo all migrations:*

```
yarn sequelize db:migrate:undo:all
```


That's it! :)
