# Rails-API

This project fully placed in Docker.

There are two ways to setup environment and run application via Docker:

1. [Visual Studio Code Remote](https://code.visualstudio.com/docs/remote/containers) - open project in VS Code.

1. Build manually from shell on any machine with docker.

## Requirements

- [Docker](https://www.docker.com/).

## Setup

0. Install `remote-containers` Visual Studio Code extensions.

    ```bash
    > code --install-extension ms-vscode-remote.remote-containers
    ```

1. Clone this repo to your machine.

    ```bash
    > git clone git@github.com:andrejreznik/rails-api.git
    ```

2. Open Visual Studio Code in `rails-api` folder.:

    ```bash
    > cd rails-api
    > code .
    ```

## Setup from shell (skip if using VS Code).

1. Clone this repo to your machine.

    ```bash
    > git clone git@github.com:andrejreznik/rails-api.git
    ```

1. Build.

    ```bash
    > cd rails-api
    > docker-compose build .
    ```

## Run application

1. To start `rails` server you need to start process in terminal:

    ```bash
    > bin/rails s -b 0
    ```

or [launch](.vscode/launch.json) application by click on `Run` -> `Run Without Debugging` <kbd>Ctrl</kbd> + <kbd>F5</kbd>

### Run in system shell

1. Start `rails` server.

    ```bash
    > docker-compose exec web bin/rails s -b 0
    ```

## Run the test suite

  ```bash
  > rspec
  ```

## Check for Rubocop offenses

  ```bash
  > rubocop
  ```
