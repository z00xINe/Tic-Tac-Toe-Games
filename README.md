# Tic-Tac-Toe-Games

A collection of four classic strategy games implemented in C++ with both console and GUI versions. This project demonstrates object-oriented design principles, game logic implementation, and user interaction handling across multiple game variants.

## Overview

This repository contains implementations of four strategic board games:
1. Pyramid Tic-Tac-Toe (3x5 triangular grid)
2. Connect Four / Four-in-a-Row (6x7 gravity-based grid)
3. 5x5 Tic-Tac-Toe (extended classic variant)
4. Classic 3x3 Tic-Tac-Toe

Each game supports two-player local multiplayer mode and single-player mode against a random-move AI opponent.

## Features

### Game Modes
- Pyramid Tic-Tac-Toe: Unique triangular board layout with restricted valid positions
- Connect Four: Gravity-based piece dropping with 4-in-a-row win condition
- 5x5 Tic-Tac-Toe: Extended grid requiring 5 consecutive marks to win
- Classic 3x3 Tic-Tac-Toe: Traditional rules with 3-in-a-row win condition

### Core Functionality
- Object-oriented architecture with reusable components
- Input validation and move legality checking
- Real-time board rendering in console interface
- Win detection for rows, columns, and diagonals
- Draw condition evaluation
- Turn-based game flow management
- Random-move AI opponent for single-player mode
- Player name registration and symbol assignment

### GUI Versions (RAD Studio)
- Native Windows GUI implementations for 3x3, 5x5, Connect Four, and Pyramid games
- Visual board rendering with clickable cells
- Interactive game state management
- Built using C++ Builder / RAD Studio framework

## Technologies Used

- C++ (C++98/03 standard compatible)
- Object-Oriented Programming principles
- Standard Template Library (STL)
- Windows Console I/O
- RAD Studio / C++ Builder for GUI versions

## Project Structure
Tic-Tac-Toe-Games/

├── Code_with_menu_for_4_games_without_GUI.cpp # Console version with all 4 games

├── 3x3_GUI_by_RAD_Studio/ # GUI implementation of classic Tic-Tac-Toe

├── 5x5_GUI_by_RAD_Studio/ # GUI implementation of 5x5 variant

├── Connect_4_GUI_by_RAD_Studio/ # GUI implementation of Connect Four

├── Pyramid_Game_GUI_by_RAD_Studio/ # GUI implementation of Pyramid Tic-Tac-Toe

├── .gitignore

└── .gitattributes


## Code Architecture

### Classes
- `X_O_Board`: Manages game board state, rendering, win/draw detection, and move validation
- `Player`: Base class for human players with name and symbol management
- `EasyPlayer`: Derived AI class implementing random move selection
- `GameManager`: Controls game flow, turn management, and win condition evaluation

### Key Methods
- `update_board(int x, int y, char mark, char Game)`: Validates and applies player moves
- `display_board(char Game)`: Renders current board state to console
- `is_winner(char Game)`: Checks win conditions specific to each game variant
- `is_draw(char Game)`: Evaluates draw conditions based on move count and board state
- `get_move(int& x, int& y, char Game)`: Handles player or AI input for next move

## Building and Running

### Console Version
1. Clone the repository:
```bash
git clone https://github.com/z00xINe/Tic-Tac-Toe-Games.git
cd Tic-Tac-Toe-Games
```
2. Compile with a C++ compiler:
```bash
g++ -std=c++98 Code_with_menu_for_4_games_without_GUI.cpp -o games
```
3. Run the executable:
```bash
./games
```

## GUI Versions

- Open the respective project folders in RAD Studio / C++ Builder
- Build and run using the IDE's native build system
- Requires Windows environment with RAD Studio installed

## Usage

1. Launch the console application
2. Enter player name when prompted
3. Select game mode:
  ```
  1: Pyramid Tic-Tac-Toe
  2: Connect Four
  3: 5x5 Tic-Tac-Toe
  4: Classic 3x3 Tic-Tac-Toe
  ```
4. Choose opponent type:
  ```
  0: Two-player local mode
  1: Play against random AI
  ```
5. Enter moves as row and column coordinates separated by spaces
6. Follow on-screen prompts until game conclusion

## Contributing

- Contributions are welcome. Suggested improvements:
-- Implement smarter AI using minimax or heuristic evaluation
-- Add network multiplayer support
-- Enhance console UI with color output or ASCII art
-- Port GUI versions to cross-platform frameworks

## License

- This project is provided for educational purposes. Feel free to use, modify, and distribute with attribution.

## Authors
- Youssef Mohamed (@z00xINe)
