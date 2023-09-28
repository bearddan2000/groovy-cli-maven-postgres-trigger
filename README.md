# groovy-cli-maven-postgres-trigger

## Description
Creates a small database table
called `dog` with an `insert update delete after` triggers.

All output normally
seen in a terminal will be in `groovy-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- groovy
- maven
  - log4j
  - postgres driver

## Docker stack
- postgres:alpine
- maven:3-openjdk-17

## To run
`sudo ./install.sh -u`
Creates groovy-srv/log

## To stop
`sudo ./install.sh -d`
Removes groovy-srv/log

## For help
`sudo ./install.sh -h`
