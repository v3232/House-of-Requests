# Blackjack Game using Deck of Cards API
This project simulates a two-player game of Blackjack using the ```Deck of Cards``` API. The game is implemented in Python, leveraging HTTP requests to manage a deck of cards, shuffle it, and draw cards for each player's turn. The simulation runs in a Jupyter Notebook environment.

## Features
* Create a New Deck: A fresh deck of cards (multiple decks combined) is shuffled at the start.
* Draw Cards: Players draw cards from the deck through API calls.
* Game Logic: The notebook contains the basic logic for playing Blackjack, including calculating card values and checking for a winner.
* API Integration: The game relies on external API requests to the ```Deck of Cards``` API for card operations, ensuring a dynamic and random gameplay experience.

## How it works
1. Deck Setup: The ```Deck of Cards``` API is used to create a new shuffled deck with 6 standard decks combined.
2. Player Turns: Players take turns drawing cards using the ```draw``` endpoint from the API. Each player starts with two cards and can choose to "Hit" or "Stay."
3. Determine Winner: The game follows standard Blackjack rules to determine the winner based on card values.

## API Details
The game uses the following endpoints from the ```Deck of Cards``` API:

1. Create Deck: ```https://deckofcardsapi.com/api/deck/new/shuffle/?deck_count=6```
2. Draw Cards: ```https://deckofcardsapi.com/api/deck/{deck_id}/draw/?count={number}```
3. Shuffle Deck: ```https://deckofcardsapi.com/api/deck/{deck_id}/shuffle/```

## Example Gameplay
1. Create and shuffle a new deck.
2. Player 1 draws two cards.
3. Player 2 draws two cards.
4. Players take turns drawing additional cards ("Hit") or staying with their current hand.
5. The game ends when one player wins by either getting Blackjack, or having the highest score under 21 without going bust.
