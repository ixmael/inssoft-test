# Innsoft backend test
This backend only register new users using [Nest](https://github.com/nestjs/nest) framework.

## Setup

### Database
Before to run the migrations, you have to create a new database. Once you have the database, you have to initialize the database with the migrations placed in *migrations* path. As was required, this use **Postgres**.

I use [go migrate](https://github.com/golang-migrate/migrate) because is more simple that **sequelize** and this gives an error.

```sh
migrate -database postgres://USER:PASSWORD@localhost:5432/DATABASE?sslmode=disable -path migrations up
```

### Installation

```bash
$ yarn install
```

## Running the app

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev

# production mode
$ yarn run start:prod
```

## Test

```bash
# unit tests
$ yarn run test

# e2e tests
$ yarn run test:e2e

# test coverage
$ yarn run test:cov
```
