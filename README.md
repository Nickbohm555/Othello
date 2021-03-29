# Othello

WHAT IS THIS ?
---------------
This project is a Graphical User Interface of the board game Othello. The rules of Othello are as follows: 

Othello involves play by two parties on an eight-by-eight square grid with pieces that have two distinct sides. Pieces typically appear coin-like, with a light and a dark face, each side representing one player. The goal for each player is to make pieces of their colour constitute a majority of the pieces on the board at the end of the game, by turning over as many of their opponent's pieces as possible. A user may only click a viable location for his/her next move. A viable location is one where the outside peices are your color and the inside pieces are the opposing players. Clicking this location flips the opposing player's peices to your color.

I added a twist to the game. Instead of playing against another User, I made an AI Computer Player that would choose it's own move based off off evaluating which would be the most optimal move. I chose an 'optimal move' to be one where the most pieces are flipped over to the Computer Player's color. 

For the User, you must choose a specific spot on the board that is a viable move when it is your turn or nothing will happen. When it switches to the CP turn, you (the user) must click anywhere on the board to activate the Computer Player's move. When you run out of spots to choose from, you can end the game by clicking the 'GAME OVER' button on the top which calculates who has more coins on the board and tells the user who won.

WHY DID I MAKE THIS?
---------------------
I made this game because I have always enjoyed playing Othello against my grandpa at home. In order for me to practice, I needed to play against a Computer Player, so I coded a CP to play against me. It also helped me understand Object Oriented Programming and design better.

HOW DO I USE THIS?
-------------------
In order to Compile this code, you have to run it in eclipse or another Java IDE since it is all coded in Java. Make sure to run the main method ('MyOthello') for the code to begin or else it won't compile.

OPTIMAL DESIGN CHOICES
-----------------------
In order to make the Code for this project cleaner, I split it up into several classes which I could conceptualize easier. I had 'MyOthello' class which brought all my classes together, I had my 'Square' class which created the squares of the gameboard, I had a 'GameBoard' class which was where I created my Graphical User Interface and Repainted after each move, I had my 'GameMouseListener' class which implemented the MouseListener class that told me where exactly on the screen was clicked, and lastly I had my 'ComputerPlayer' class which scoped through each open spot on the board and 1) checked if it was a viable spot and 2) checked if it was the optimal move to make.

FUTURE IMPROVEMENTS
-------------------
There are mainly two things that I would improve. The first would be to add more criteria of what an 'optimal move' for the Computer Player is. I would possibly come up wih an equation that takes into account whether a certain peice was a corner peice vs how many coins it would flip. The second thing I would fix is a few bugs in the program. For some reason, the computer player is only able to start it's turn if I, the user, chooses a very specific first move. I would change this to activate the CP for any first move.
