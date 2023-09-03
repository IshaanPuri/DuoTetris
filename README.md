# DuoTetris
Engineered a 2 player competitive Tetris game using objected oriented principles in C++

A two player turn based Tetris game that follows Object Oriented Programming fundamentals. Collaborated with 2 team members to create Competitive Tetris as our final project for a course.

Due to academic integrity concerns the source code for this project is not made publically available, however below I have attached several screenshots of the game and would be happy to provide it upon request.

Incorporated Observer, Factory method, Decorator, and Model View Controller design patterns. It also used techniques such as Polymorphism, RAII and single responsibility principle.

## Unified Modeling Language (UML) Diagram:

<img width="1080" alt="UML" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/91f0ee65-b585-43bc-8b5e-1bab2fd02cb3">

## Graphical and Text mode screenshots:

<img width="1006" alt="Scoreboard_Graphic" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/a7980854-35a5-48c5-b9e9-2648b84f3da1">


<img width="334" alt="Scoreboard_Text" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/706bdfcf-fc0a-434e-b69e-7f85b432635b">

Below are the visual examples of the game's major features. Textual representations have been omitted for clarity but can be found in the Game_screenshots folder.

## Leveling up feature:

Each player can level up or down to adjust the probabilities of harder or easier blocks spawning, and presence of debuffs, to increase points they earn once they clear row(s). There are 4 levels all of which leverages the Factory method design pattern.

<img width="1012" alt="Level_Graphic" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/d88da7f2-4628-46b6-ae86-bef3cca6ec1d">

## Movement features:
All seven block types can be moved in all directions except up, rotated counter clockwise and clockwise all with appropriate collision detection. 
Below is a demonstration of the rotation feature:

<img width="1012" alt="Level_Graphic (1)" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/147b08db-90b6-4fda-a21d-afc2250b6557">
<img width="1014" alt="Movement_Graphic" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/a8566df2-c7bf-4b25-bec0-239bcf26200e">

## Score:

After filling up row(s) they are cleared and points are added into the player's score through the following equation: Points_added = (Current_level + Rows_cleared) ^ 2

<img width="1006" alt="Scoreboard_Graphic (1)" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/329dc805-e6b9-46d8-ad58-6a4a17522fa7">
<img width="1010" alt="Scoreboard_Graphic_2" src="https://github.com/IshaanPuri/DuoTetris/assets/56935073/8bfd27d4-23da-4562-ba44-d79e512eced1">

In this case it was: Points_added = (3+1)^2 = 16

There is also a CLI interface that lets you pass in files containing the block sequences for each player, starting level, game mode, and randomization seed.

