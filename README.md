# Ataxx

## Overview
**Ataxx** is a two-person strategy game with the goal of populating the board with your colour dots. A **legal move** consists of **adding** a dot of your colour adjacent to an existing dot (_extend_), or **moving** an existing dot to a non-adjacent square that is not more than two rows and two columns away (_jump_). Moving to a square adjacent to the opponent's colour results in it being changed to your colour. Additionally, the board can contain blocks that cannot be moved to due to preset **obstacles**. The game ends when neither player can make any moves, or when 25 consecutive jumps across both players has been played. In that case, the board is evaluated and the winner is the player with the most number of dots (or a _tie_ in the case of an equal number of dots).

I created a command-line version of Ataxx defining the **board**, **obstacles**, and **legal moves**. I also implemented commands such as `undo`, `help`, `new`, `quit`.

## AI Opponent
I also implemented an AI that can be played against. This AI is able to find a **forced win** that is within four moves of any given position. I was able to accomplish this by implementing the **MiniMax algorithm** on game-trees, and optimizing move search using **Alpha-Beta pruning**.

## Acknowledgements
This project was part of my coursework in UC Berkeley's CS61B Data Structures course. More details regarding the documentation of this project can be found [here](https://inst.eecs.berkeley.edu/~cs61b/sp22/materials/proj/proj2/index.html). Since this is a class project, I cannot post the code publicly, but can make it available upon request.
