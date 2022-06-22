# CPPND: Capstone Snake Game Example

This is my Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). The code for this repo was inspired by [this](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) excellent StackOverflow post and set of responses.

## Tasks implemented

  1. Allowed users to enter their names and save it in a text file with their scores, so that one can get the top score
  2. Allowed the user to select the initial speed (Slow - Fast)
  3. Added a peacock as a moving obstacle to the game
  4. Displayed More than one type of food in the game
  5. Included anaconda (or a python snake) to the game and allowed the computer to control it using **A* search algorithm**

## Task 1
1. Created scoreCard.h and scoreCard.cpp with necessary data structures and its attributes, methods, constructors, destructors etc.
2. In the main(), an object of type scoreCard is created to invoke the constructor of Struct scoreCard
3. Read/Write to file operations are implemented to sort score and display top scores etc.

Input(s) - player name



## Task 2
1. Created startSpeed.h and startSpeed.cpp with necessary data structures and its attributes, methods, constructors, destructors etc.
2. In the main(), an object of type startSpeed is created to invoke the constructor of Struct startSpeed
1. Changed score type from int to float
2. Changed the arguments list of Game::Game(...) to set a new private attribute named initSpeed with a user selected start speed value and modified Game::Update() to  set different score increments for different modes (slow-speed)
4. Snake::Snake(...) arguments list changed, attribute Snake::speed gets initialised according to user's speed choice instead of default initialisation with 0.1f
5. Renderer::UpdateWindowTitle(..) arguments list modified and sstream library is used to display float with a score value of single precision.

Input(s) - User's choice of speed
<img src="snake_game.gif"/>

<!-- The Capstone Project gives you a chance to integrate what you've learned throughout this program. This project will become an important part of your portfolio to share with current and future colleagues and employers.

In this project, you can build your own C++ application or extend this Snake game, following the principles you have learned throughout this Nanodegree Program. This project will demonstrate that you can independently create applications using a wide range of C++ features. -->

## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  >Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source. 
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.


## CC Attribution-ShareAlike 4.0 International


Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
