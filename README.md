# Slack + Shopify Workflow

## Introduction

The project will consist of building a a mini workflow engine that listens for new Shopify orders, and when orders are placed, triggers off a Slack alert if the order total exceeds $100.

## User Stories

- As a client, to have page where to authenticate pages.

- As a client, I want to get a notification when shopify order exceeds $100 or more.

## Proposed Solution

### Stack

- NodeJS
- React
- Typescript
- MongoDB


## Setup and Run Backend

Every slack and shopify token must be set in the `.env` for backend to work. Also, must be configured and connected to a mongoDB. To run the backend locally:

```
cd /path/to/backend

# Create and copy example .env
cp example.env .env

# Install packages
npm i

# Run backend
npm run dev
```

## Setup and Run Frontend

To run a local server use the command

```
cd /path/to/frontend

# Create and copy example .env
cp example.env .env

# Install packages
npm i

# Run backend
npm run start
```

### TESTS

- TODO

### TODO

- Dockerize
- Better authentication. Maybe have a refresh token and access token
- Shopify better verification with state and hmac [https://shopify.dev/apps/auth/oauth#how-the-installation-flow-works]
- Tests for backend and frontend
- Better account handle with slack and shopify
- Frontend improve token handling. We could have an axios interceptor for response `401` and request a new token.
- Have a Frontend task to ask for new token every x time
- Create a base any type of integrations
