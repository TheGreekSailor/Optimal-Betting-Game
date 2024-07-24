# Optimal-Betting-Game

## Motivation behind project

This is an attempt to solve a game-theory style betting problem which involves probabilistic reasoning and optimization of betting at each round by manually calculating the derivatives and finding the bet that maximizes the players EVs

## Description

This mini-game simulates a multi-round betting game between two players with non-linear multiplier payouts. 

The payout structure is as follows:

If the outcome is 1 or 2, Player A wins and receives a payout based on their bet.
If the outcome is 3 or 4, Player B wins and receives a payout based on their bet.
If the outcome is 5 or 6, both players lose their bets.

Each player has an initial amount of W1 and W2 dollars, respectively. The game lasts for n rounds. Players can bet up to 10% of their net worth at every round. 

The payout multiplier function is:

Player A's payout multiplier is k_A(bet_A) = 1 + log(1 + bet_A) where bet_A is the bet amount of player A at each round
Player B's payout multiplier is k_B(bet_B) = 2 + sqrt(bet_B) where bet_B is the bet amount of player B at each round

The task is to determine the optimal betting strategy at every round for players A and B using probabilistic reasoning and optimization techniques
