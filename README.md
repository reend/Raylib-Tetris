# Tetris Game

This project is a simple implementation of the classic Tetris game using the Raylib library for graphics rendering. The game is designed to be cross-platform and can be compiled and run on Windows, macOS, and Linux.

## How the Program Works

The Tetris game consists of falling blocks of different shapes that the player must arrange to form complete rows. When a row is completed, it is cleared from the grid, and the player earns points. The game continues until the blocks reach the top of the grid, resulting in a game over.

### Key Features

- **Block Movement**: The player can move blocks left, right, and down, as well as rotate them.
- **Score System**: Points are awarded for clearing rows, with more points for clearing multiple rows at once.
- **Game Over Detection**: The game ends when new blocks can no longer be placed on the grid.

### Controls

- **Left Arrow**: Move block left
- **Right Arrow**: Move block right
- **Down Arrow**: Move block down faster
- **Up Arrow**: Rotate block

## Project Structure

The project is organized into several files, each responsible for different aspects of the game:

- **`src/main.cpp`**: The entry point of the application. It initializes the game window, handles the main game loop, and manages rendering.
- **`src/game.h` and `src/game.cpp`**: Define the `Game` class, which manages the game state, including the grid, current and next blocks, and score.
- **`src/grid.h` and `src/grid.cpp`**: Define the `Grid` class, which represents the game grid and handles operations like clearing full rows and checking cell states.
- **`src/block.h` and `src/block.cpp`**: Define the `Block` class, which represents a Tetris block, including its shape, position, and rotation.
- **`src/blocks.cpp`**: Contains the definitions of different Tetris block shapes (I, J, L, O, S, T, Z).
- **`src/colors.h` and `src/colors.cpp`**: Define the colors used for different blocks and the grid.
- **`src/position.h` and `src/position.cpp`**: Define the `Position` class, which represents the row and column of a block's cell.

## Build and Run

To build and run the game, you need to have Raylib installed on your system. The project uses a Makefile for building the application.

### Development Environment

The project is set up to be used with Visual Studio Code, with configuration files provided for building and debugging the application on different platforms.

- **`.vscode/tasks.json`**: Defines tasks for building the project in debug and release modes.
- **`.vscode/launch.json`**: Configures the debugger for running and debugging the application.
- **`.vscode/c_cpp_properties.json`**: Sets up include paths and compiler settings for IntelliSense.
