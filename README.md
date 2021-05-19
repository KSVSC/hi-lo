# HighLow
This is an implementation of decentralised app.

# Usage
1. Clone the repository `git clone https://github.com/KSVSC/hi-lo`
2. `cd hi-lo && npm i`
3. `truffle build`
4. `cd app && npm i`
5. Run the backend server `go run Backend.go` from the `backend/` directory
6. Run the blockchain test net `truffle develop` and use `deploy` in the interactive CLI to deploy the contracts
7. Run the front-end server `npm start` from the `app/` directory

Enjoy the game!

# Details
The UI of the game was built with `Two.js` (https://two.js.org/) backend (deployed on blockchain) was written in Solidity and a minimal Golang server is used as a backend for handling the contract addresses.


## Game Implementation

- It is a multiplayer game.
- Once the game is deployed we see a open card with some value.
- Players can register to the game by betting their commitments High/Low.
- With an interval of every 30 sec the new cards are released.
- After the next card is revealed, all the players who bet their commitment for previous card reveal their commitments.
- Players with right bet recieve money.
