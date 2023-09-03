# DuoTetris
Engineered a 2 player competitive Tetris game using objected oriented principles in C++

A two player turn based Tetris game that follows Object Oriented Programming fundamentals. Collaborated with 2 team members to create Competitive Tetris as our final project for a course.

Due to academic integrity concerns the source code for this project is not made publically available, however below I have attached several screenshots of the game and would be happy to provide it upon request.

Incorporated Observer, Factory method, Decorator, and Model View Controller design patterns. It also used techniques such as Polymorphism, RAII and single responsibility principle.

Unified Modeling Language (UML) Diagram:
We created a UML diagram to serve as a guideline for developing our program.

UML not rendering

Graphical and Text mode screenshots:
UML not rendering UML not rendering

Below are the visual examples of the game's major features. Textual representations have been omitted for clarity but can be found in the Game_screenshots folder.

Leveling up feature:
Each player can level up or down to adjust the probabilities of harder or easier blocks spawning, and presence of debuffs, to increase points they earn once they clear row(s). There are 4 levels all of which leverages the Factory method design pattern.

UML not rendering

Movement features:
All seven block types can be moved in all directions except up, rotated counter clockwise and clockwise all with appropriate collision detection.

Below is a demonstration of the rotation feature: UML not rendering

UML not rendering

Score:
After filling up row(s) they are cleared and points are added into the player's score through the following equation:

Points_added = (Current_level + Rows_cleared) ^ 2

UML not rendering

UML not rendering

In this case it was: Points_added = (3+1)^2 = 16

There is also a CLI interface that lets you pass in files containing the block sequences for each player, starting level, game mode, and randomization seed
