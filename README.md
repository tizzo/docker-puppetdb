# Docker PuppetDB

A simple puppetdb docker container for pupetdb.

## Usage:

    git clone https://github.com/tizzo/docker-puppetdb.git
    cd docker-puppetdb
    docker build .
    docker run --name puppetdb-postgres -e POSTGRES_PASSWORD=puppetdb -e POSTGRES_USER=puppetdb -d postgres
    docker run -d -P --link puppetdb-postgres:postgres puppetdb

