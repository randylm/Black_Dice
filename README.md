# Black_Dice


## Introduction
We designed a new game named Blackdice by making some modification on the famous BlackJack card game. Based on the new game rule, we frame it as a reinforcement learning problem and applied Monte Carlo method to evaluate different policies.

## Two main differences with BlackJack
If a player’s hand is less than 12, then player is required to draw another card.
If a player’s hand is greater than or equal to 12, then player can decide whether to roll a die. If the player decides to roll a die, then the value from the die is added to the player’s hand. Player can roll a die multiple times until busted.
The rest of the Blackdice is the same as the standard Blackjack including the dealer hits on soft 17.

## Reinforcement Learning Framework
- Based on the rules above, we can frame this game in the following way:
- Agent: the player
- Environment: a deck of cards and a die
- State: the value in player’s hand
- Reward: 1 for winning, -1 for losing, 0 for tie
- Action: stay or roll a die
