# RubiksCube-TwophaseSolverFiveFaces
## Overview 
This project is a modified version of the main RubiksCube-TwophaseSolver project and solves the Rubiks Cube in less than 22 moves on average without turning the back face. SInce the possibilities for symmetry reductions are reduced in this case the pruning tables are about 4 times the size compared to the main project and also the time to create the tables is about 4 times larger. 

## Usage
There are several tables which must be created on the first run. These need about 243 MB disk space and it takes from about 2 to 24 hours to create them, depending on the hardware. Usually you start the cubesolving server which listens on a port of your choice and which accepts the cube definition string and returns the solving maneuver. The module example.py gives detailed examples how to start the server and a simple GUI-interface which interacts with the server. You can run the example file with

"python example.py" or eventually "python3 example.py"

Make sure that you use Python 3.4 or higher and you have the numpy package installed. 
