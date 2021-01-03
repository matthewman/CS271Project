# CS271 Introduction to Artificial Intelligence Project

## Overview

This project contains the implementation of Q-Learning in Python to solve the [Sokoban problem](https://en.wikipedia.org/wiki/Sokoban).

The input files for our project are located in the `/Input` directory. The given input files for are `sokobanXX.txt`, and the `inputXX.txt` are the corresponding visualizations.

## Run Instructions

### Q-learning program

To run the Q-learning program:

1. Download and install [Jupyter Notebook](https://jupyter.org/).
2. Open the `CS271Project.ipynb` file.
3. Specify the specific Sokoban problem input file in the 3rd cell of the notebook.
4. Select `Cell->Run All`.

After completion, the program outputs the length of action sequence it found and the corresponding action sequence.

## Additional Notes

### Input files

Input files contains 5 lines

1. Line 1: sizeH sizeV
2. Line 2: nWallSquares wall1X wall1Y wall2X wall2Y ...
3. Line 3: nBoxes wall1X wall1Y wall2X wall2Y ...
4. Line 4: nStorages wall1X wall1Y wall2X wall2Y ...
5. Line 5: playerX playerY

### Input visualizations

The input visualizations files are defined as follows:

- `@` represents the player's location.
- `#` represents a wall location.
- `*` represents a location of a storaage with a box .
- `$` represents a location of a box (but not a storage).
- `.` represents a location of a storaage (without a box).

### Input conversion

For experimental purposes, we have created some custom Sokoban problems as `customSokoban_.*.txt` inside the `/Input` directory. The corresponding visualizations are named without the `customSokoban_` part.

We also added the `/Input/InputConversion.ipynb` notebook file, which converts a visual input into a text input that our Q-learning program uses.
