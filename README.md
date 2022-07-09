# AI-based-Checkers Game

Have created an agent using AI techniques to play the game of checkers intelligently. We have an 8x8 board and two opponents play against each other where each opponent has 12 pieces at the beginning of the game. It is a two person zero-sum game. Minimax or Minimax algorithm is best suited for such types of games. In this implementation, the human player can play against the intelligent AI player. However, due to the large number of possible moves at any given point in the game, traversing the game tree for higher depths becomes extremely slow, which is why in addition to Minimax, we also implemented Alpha Beta pruning to considerably speed up our algorithm. 
The greater the depth of the minimax tree, the better the move made by the AI. The evaluation criteria we used to calculate the goodness of a move was that the ego player will prioritize to maximize the number of its own pieces and minimize the number of pieces of the opponent player. We also incentivize maximizing the number of kings for the max player and minimize the number of kings for the min player.
The game ends when either only the pieces of one player are left on the board or when the player who is supposed to go next is locked in and can not make any further moves.



# Steps to run the application

## Step 1

cd into the folder named 'frontend' and then run the command 'npm install'. 

## Step 2

cd back into the main folder named 'AI-based-Checkers' and run the following commands in order:

- python -m venv venv
- venv\Scripts\activate.bat
- pip install -r requirements.txt


## Step 3

We will need to run both flask and React server. 

### Running Flask Server

cd into the main folder named 'AI-based-Checkers' and run the command 'flask run'. This will run the flask server

### Running React Server

cd into the folder named 'frontend' and run the command 'npm start'. This will run the React server. 