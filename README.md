[![CI](https://github.com/emtiajium/query-comparison/actions/workflows/ci.yml/badge.svg)](https://github.com/emtiajium/query-comparison/actions/workflows/ci.yml)

# What is this repository for?

[Demystifying ORM Queries: The Search for Optimized Queries](https://dev.to/emtiajium/demystifying-orm-queries-the-search-for-optimized-queries-2lbk)

# How to Run

###### Prerequisites

➜ Install Node 18.13.0 using [nvm](https://github.com/nvm-sh/nvm)

➜ Install [docker](https://docs.docker.com/get-docker/) and [docker-compose](https://docs.docker.com/compose/install/)

###### Clone the repo and install all dependencies

➜ `git clone git@github.com:emtiajium/query-comparison.git`

➜ `cd query-comparison`

➜ `npm install`

###### Run backing services

➜ `docker-compose up -d`

###### Create the configuration

➜ `npm run create:env`

###### Synchronize model changes into the database

➜ `npm run migration:run`

###### Insert data

➜ `bash scripts/db-restore.bash`

###### Run tests

➜ `npm run test`

###### Start the development environment

➜ `npm run start:dev`

## Generate new migration script after changing the entity class(es)

➜ `npm run migration:generate migrations/<file-name>`

## Remove backing services

➜ `npm run clean:docker-containers`

## Change Logs

-   `0.0.1`: --- ---
