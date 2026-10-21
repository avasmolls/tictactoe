# Tic-Tac-Toe | React Application

A React-based Tic-Tac-Toe project demonstrating component-based architecture, event handling, and reusable UI elements. The application provides a 3×3 game board designed for two-player gameplay using X and O.

## Project Overview

This project explores fundamental React development concepts through a classic Tic-Tac-Toe interface.

The application is organized into reusable functional components that separate the overall application, game interface, board layout, and individual squares.

The current implementation establishes the board layout and click-event handling, providing a foundation for implementing game state management and complete gameplay functionality.

## Features

### Currently Implemented

- **Interactive Game Board:** Displays a 3×3 grid consisting of nine clickable squares.
- **Reusable Components:** Uses separate React components for the application, game, grid, and individual squares.
- **Event Handling:** Processes square clicks through callback functions and identifies the selected square.
- **Turn Display:** Displays the current player indicator, initially set to X.
- **Player Styling:** Defines distinct text colors for X and O.
- **Game Controls:** Includes a New Game button interface.

### Planned Functionality

- Alternate turns between X and O.
- Store player moves using React's `useState` hook.
- Prevent players from selecting occupied squares.
- Reset the board when New Game is clicked.
- Detect winning combinations.
- Identify draws when the board is full.

## Technologies Used

- **React 18** — Component-based user interface development
- **JavaScript (ES6+)** — Functions, arrays, and event handling
- **HTML5** — Application structure
- **CSS3** — Grid layout, typography, and player styling
- **Parcel** — Development server and application bundling
- **Node.js / npm** — Dependency management

## Component Architecture

The application is organized into four primary React components.

### App (`App.js`)

- Serves as the root application component.
- Renders the Game component.

### Game (`Game.js`)

- Defines the game board's initial values.
- Displays the game title, turn indicator, and New Game button.
- Provides the square-click callback.
- Serves as the central location for future game state management.

### GameGrid (`GameGrid.js`)

- Constructs the 3×3 game board.
- Renders nine reusable Square components.
- Receives board values and click handlers through props.
- Passes each square's index to the click handler.

### Square (`Square.js`)

- Represents
