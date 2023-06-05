## SOS

SOS game gameplay, with an AI-powered agent as one of the players

----------

SOS is a game that can be played with a pencil and paper. It is quite similar to tic-tac-toe but can have a larger grid and players in each turn can choose between “S” and“O”. Thus, the game has a much larger complexity than tic-tac-toe. While tic-tac-toe can become too predictable, SOS is guaranteed to keep players thinking about their future actions. The goal of this game is to cover the board with as many “S-O-S” formations as possible, and each formed SOS will increase the score of that particular player by 1. In SOS, there are little to no limitations for the board design. The uniqueness is in its connection with timing: the bigger the board, the longer the game will last.


<img src="SOS_game.png" style="height: 300px">

There are 4 agents are available in the gameplay
* Random Player
* User Player
* MiniMax Player
* Smart Random Player*

**Random Player** - *randomly makes moves based only on empty spaces on the board.*

**User Player** - *used for human user.*

**Smart Random Player** - *if the players opponent has an opportunity to make a "S-O-S" after the players move, the utility is one divided by the score. The more "S-O-S"s the opponent will be able to make after a certain move, the less the utility will be. Thus, the less the utility the less the chances that that move is going to be chosen.*  (Selected when MiniMax Player is selected with 0 depth)

**MiniMax Player** - *uses of MiniMax algorithm optimized by Alpha-Beta pruning technique accompanied by complex evaluation functions and scalable depth.*

The beninning of the gameplay provides a **scaleable board** size and a **scaleable depth** for MiniMax agent, if *MiniMax Alpha Beta Player* is selected.

<img src="sos_start.png" style="height: 300px">

The gameplay provides information on **percentage(%) of the nodes pruned by Alpha-Beta optimization, player scores, and current points**.

<img src="sos-demo.png" style="height: 400px">

Based on gameplay statistics, MiniMax Player wins in 95% of games against real people.


