# Install Docker

https://docs.docker.com/compose/install/

- Docker Desktop for Mac

# Instructions:

`cd Sites`

`mkdir ugorago`

https://docs.docker.com/compose/rails/

`touch Dockerfile`

`touch Gemfile`

`touch Gemfile.lock`

`touch entrypoint.sh`

`touch docker-compose.yml`

# Build the project

`docker-compose run --no-deps web rails new . --force --database=postgresql`


# reBuilding the Image

 Changes to the Gemfile or the Dockerfile, should be the only times you’ll need to rebuild.

`docker-compose build`

# Yarn

` docker-compose run web bundle exec rails webpacker:install`

# Connect the database

`docker-compose up`

## Create DB

`docker-compose run web rake db:create`


# Start/Stop/ReBuild

`docker-compose up`

`docker-compose down --build`

`docker-compose up --build`

