# RL-BlackjackGame
Using Monte Carlo Tree Search (Reinforcement Learning) for the game of Blackjack (mcts player, timid player, basic strategy player, console player). The MCTS player uses the UCB value to make the trade-off between exploration and exploitation. We pick the most promising nodes/actions based on that UCB value. Formula is *UCB = sumOfExpectedValues/currNodeVisitations + c \* sqrt(ln(parentNodeVisitations)/currNodeVisitations)* where we used **c=2**. Lower **c** value yields more exploitation, higher **c** value yields higher exploration.

## command to run the program: `python blackjack.py`

You can use optional flags like:
* `-q` (for quiet output without all the print statements)
* `-d` (for the deck types: {default, odd, even, high, low, random}) *example:* `-d odd`
* \<player-type\> (which can be `mcts`, `timid`, `basic`, `console`)


### example: `python blackjack.py -q -d even mcts`
where you specified for mcts player to play against the dealer with an even deck!
