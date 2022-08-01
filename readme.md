# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

- [Welcome to the Anythink Market repo](#welcome-to-the-anythink-market-repo)
  - [Development](#development)
  - [First setup](#first-setup)

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

<!-- **[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_ -->

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Welcome to the Anythink Market repo](#welcome-to-the-anythink-market-repo)
  - [Development](#development)
  - [First setup](#first-setup)

<!-- /code_chunk_output -->
<!-- /code_chunk_output -->
Make sure you have docker install in your system download from here [install docker](https://docs.docker.com/get-docker/).

- You can verify docker is ready by running the following commands in your terminal: `docker -v` and `docker-compose -v`
- Next run `docker-compose up` from the project root directory,this will load Anythink's backend and frontend.
- If Docker is working correctly, the backend should be running and able to connect to your local database.
  - Let's test this by pointing your browser to http://localhost:3000/api/ping

- Now, let's check frontend and make sure it’s connected to the backend.
  - If everything is working properly, you’ll be able to create a new user on http://localhost:3001/register
  - Create one (choose a cool nickname and everything) and you’ll be able to move to the next step.
- Just make sure that you run all scripts in the next quests on one of the containers created by `docker-compose up`.  Also, you can use `docker exec` to run commands on a running container.

It looks like your environment is ready! 😀