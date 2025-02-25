# Authenticate Users With SAML Example Repository

This repository accompanies the [FusionAUth guide to authentication users with SAML](https://fusionauth.io/docs/lifecycle/examples/authenticate-users-with-saml)

## How To Run

- Clone this repository using `git clone` or by downloading and unzipping it.

  ```sh
  docker compose up

  # in a new terminal
  cd app
  docker run --platform=linux/amd64 --rm -v ".:/app" -w "/app"  node:23-alpine3.19 sh -c  "npm install"
  docker run --platform=linux/amd64 --rm -v ".:/app" -w "/app" --name app --network faNetwork  -p 3000:3000 node:23-alpine3.19 sh -c  "npm run start"
  ```
- Log in to FusionAuth at `http://localhost:9011` with `admin@example.com` and `password`.
- Log in to Changebank at `http://localhost:3000` with `richard@example.com` and `password`.
