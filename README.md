# logmein-test

Hi, this is my solution for LogMeIn Senior Java Developer position. I've implemented this project in Eclipse, which currently is my primary IDE.

## Used technologies

- Java 8
- Maven 3
- Google Guava
- Apache Commons
- For shuffling: Only java.util.* :)

## Implemented functions

The following list shows the status of the new functions ([+] is ready, [-] is not):

- [+] Create and delete a game
  - PUT /game
  - GET /game/{id}
  - DELETE /game/{id}
- [+] Create a deck & add it a deck to a game
  - PUT /game/{id}/addDeck
- [+] Add and remove players to a game
  - PUT /player
  - DELETE /player/{id}
- [+] Deal cards to a player
  - POST /game/{id}/deal/{playerId}
- [+] Get the list of cards for a player
  - GET /player/{id}
- [+] Get the card values for all players
  - GET /game/{id}/players
- [+] Get undealt card count
- [+] Get card count with an order
- [+] Shuffle game deck
  - POST /game/{id}/shuffle

## Build

> mvn clean install

## Soap UI Project

To test the functions, I've created a Soap UI project. 

> LogMeIn-homework-soapui-project.xml