# Tic Tac Rails

This is a React on Rails project to exemplify multiple servers working together to play a simple game of Tic Tac Toe.

The client prompts the game and displays the results. The goals for this exercise are to allow two versions of play:

- **1. Constant Updates:**
All moves go through the client. This means that the client keeps track of the state of the game in the front end, and requests each new move until the game is over. The state of the game is updated until either server wins.

- **2. Final Results Only:**
The client signals to a random choice of either server to start the game, then they report their moves back and forth to each other, until either wins. The final winner is reported to the client, and the results are finally updated.

## Running it Yourself:

To run an instance of Tic Tac Rails, clone this repo and, on the command line, open four seperate tabs. In the first tab, navigate into `./tic-tac-rails-client` and run `rails s -p 3000`. In the second, also navigate into `./tic-tac-rails-client` and run `yarn start`. In the third, navigate into `./tic-tac-rails-server` and run `rails s -p 3001`. In the fourth, also navigate into `./tic-tac-rails-server` and run `rails s -p 3002`.

In your browser of choice, open `localhost:3000`.