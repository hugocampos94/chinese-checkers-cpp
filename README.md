# chinese-checkers-cpp

## Description
This is a console version of the chinese checkers game.

Follow the instructions to play, you can start a game for 2,3,4,5 or 6 players.
After each move the current status of the board will be printed in the format `{player number}{RowID}{ColumnID}`, if the position is empty no player number will be shown in that space of the board.

The app works in a loop. Once a game finishes the next one can be started right away.

## Structure

The structure of the project is as follows:

***Board.h/Board.cpp***: Encapsulates the board status, keeps track of players.

***Coordinate.h/Coordinate.cpp***: Class used to represent a position in the Board.

***Game.h/Game.cpp***: Utility class that defines methods to retrieve user input and contains the entry point of the application.

***Movement.h/Movement.cpp***: Defines the move operations that can be performed on a Coordinate of the Board.

***Player.h/Player.cpp***: Class used to encapsulate player info.

***PlayerPositions.h/PlayerPositions.cpp***: Defines the Start and End positions that can be assigned to each player.

## Compilation

This project uses CMake. The following commands will create and run the executable

```
mkdir build
cd build
cmake ..
make
./chinese-checkers-cpp
```

## Udacity Rubric Points

**The project demonstrates an understanding of C++ functions and control structures.**
- *Files:*
  - Game.cpp Line 94
  - Board.cpp Line 140

**The project accepts user input and processes the input.**
- *Files:*
  - Game.cpp Lines 12,38,58

**The project uses Object Oriented Programming techniques.**
- *Files:*
  - All header files declare classes, all cpp files define the classes.

**Classes use appropriate access specifiers for class members.**
- *Files:*
  - All header files declare public/private members

**Class constructors utilize member initialization lists.**
- *Files:*
  - Board.cpp Lines 46, 53
  - Movement.cpp Line 8
  - Player.cpp Line 7

**Classes encapsulate behavior.**
- *Files:*
  - Board.cpp
  - Player.cpp
  - PlayerPositions.cpp

**The project makes use of references in function declarations.**
- *Files:*
  - Board.cpp (Most functions in this class use)