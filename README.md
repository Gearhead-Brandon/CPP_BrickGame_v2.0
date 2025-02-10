# BrickGame Snake - Snake Game Implementation in C++

## Contents

1. [Introduction](#introduction)
2. [General Information](#general-information)
   - [Snake](#snake)
3. [Project Requirements](#project-requirements)
   - [Part 1: Main Task](#part-1-main-task)
   - [Part 2: Bonus - Scoring and Game Record](#part-2-bonus-scoring-and-game-record)
   - [Part 3: Bonus - Level Mechanics](#part-3-bonus-level-mechanics)

## Introduction

In this project, you will implement the classic Snake game in C++ using object-oriented programming. The project involves developing two components: a library for the game logic and a desktop GUI. The library must be integrated with the console interface from BrickGame v1.0 and fully support the Snake game, alongside the Tetris game from the previous project.

## General Information

### Snake

The game involves a snake controlled by the player to eat apples and grow longer, while avoiding walls and itself. The goal is to reach a maximum length of 200 "pixels" or avoid losing by bumping into obstacles.

- The game logic should be formalized using a **finite-state machine (FSM)**.
- **MVP**  pattern are  to separate concerns and improve maintainability.

## Project Requirements

### Part 1: Main Task

- Implement the game logic and desktop GUI using C++17.
- Use a finite-state machine for game logic.
- The game library code should be placed under `src/brick_game/snake`.
- The GUI code should go under `src/gui/desktop`.
- The program must be implemented using the MVC pattern, with no business logic in the view.
- The snake moves automatically, grows after eating apples, and the game ends if it crashes or reaches the max length of 200 units.
- Controls: Arrow keys to change direction, a key to speed up the snake.
- The game field is 10x20 "pixels", and the snake starts with a length of 4 "pixels".

### Part 2: Bonus - Scoring and Game Record

- Implement scoring and track the maximum score across sessions.
- The score is updated each time the snake eats an apple.
- Store the maximum score in a file or database.

### Part 3: Bonus - Level Mechanics

- Increase the game level every time the player earns 5 points, making the snake move faster.
- The game has a maximum of 10 levels.