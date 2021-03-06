# Trade bot

[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

![Node.js CI](https://github.com/danielivert/trading-bot/workflows/Node.js%20CI/badge.svg)

## Description

Trade bot using Alpaca as a bropker

## Installation

```bash
$ yarn
```

## Running the app

```bash
# development
$ yarn start

# watch mode
$ yarn start:dev

# production mode
$ yarn start:prod
```

## Test

```bash
# unit tests
$ yarn test

# e2e tests
$ yarn test:e2e

# test coverage
$ yarn test:cov
```

## Get started

- Create an account on [Alpaca.markets](https://alpaca.markets)
- Go to `paper trading` on the left navigation
- Obtain your API keys on that view.
- Add both `ALPACA_API_KEY` & `ALPACA_SECRET_KEY` to the .env variables
- Add the algorithm you want to try on the .env file. Example: `BOT_TYPE=LONG_SHORT`
- Run the app

## Environmental variables

Please have a look at .env.sample to get started

## BOT_TYPE

There are two different types of algorithms

- `MEAN_REVERSION`
- `LONG_SHORT`

## MEAN_REVERSION

This algorithm requires an additional env variable:

```
MEAN_REVERSION_STOCK
```

This variable should have the value of the name of the stock. Example Apple = AAPL

## Disclaimer

This project is done to test different trading strategies in a paper trading environment. If you want to try this to do live trading do it by your own risk.
