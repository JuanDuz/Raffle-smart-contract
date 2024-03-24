# Raffle smart contract

Users can enter the raffle with a fee, every raffle interval a winner from the players will be selected and get the ether.

## Project overview

The objective of this project was to learn oracle interaction with Chainlink.

Using chainlink VRF & Chainlink automation.

- Chainlink VRF -> Randomness (In order to get a winner)
- Chainlink automation -> Time based trigger (In order to continously pick a winner from participants)

## Use cases

1. Users can enter a raffle by paying a ticket.
   The tickets fees are going to the winner during the draw.

2. After X period of time, the lottery will automatically draw a winner.

### Tests

```shell
$ make test
```

### Deploy

local:
```shell
$ make anvil
```
```shell
$ make deploy
```

To sepolia testnet:
```shell
$ make deploy ARGS="--network sepolia"
```
