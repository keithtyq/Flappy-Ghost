# Flappy Ghost

## Description

Flappy Ghost is a simple 2D side-scrolling game inspired by Flappy Bird, developed in Unity using C#. The player controls a ghost that must navigate through moving obstacles (pipes) by flapping to stay in the air.

## Features

- **Flapping Mechanic**: Press spacebar to make the ghost flap and stay in the air.
- **Obstacle Movement**: Pipes move from right to left.
- **Scoring System**: The player earns points by successfully passing through pipe gaps.
- **Game Over Condition**: Collision with pipes or exceeding screen bounds ends the game.
- **Restart Functionality**: The game restarts upon failure.
- **Sound Effects**: A ding sound plays upon scoring a point.

## Scripts Overview

### 1. BlockMoveScript

- Moves obstacles (pipes) from right to left at a fixed speed which can be adjusted easily.
- Destroys pipes once they move past a defined "dead zone" to free up memory space.

### 2. GhostScript

- Controls the player's movement using Rigidbody2D.
- Handles player input to flap.
- Checks for collisions with pipes or screen boundaries to trigger a game over.

### 3. LogicScript

- Manages the game's score and updates UI.
- Triggers game over screen upon failure.
- Provides a function to restart the game.
- Plays a sound effect upon scoring a point.

### 4. PipeMiddleScript

- Detects when the ghost successfully passes through a pipe gap.
- Calls the addScore function in LogicScript to increase the player's score.

### 5. PipeSpawnScript

- Periodically spawns new pipes at a random height within a defined range.
- Ensures continuous gameplay by generating new obstacles.

## How to Play

- Press Spacebar to make the ghost flap.
- Navigate through the gaps between pipes.
- Avoid hitting the pipes or going off-screen.
- Earn points by passing through pipes.
- If you collide with an obstacle, the game ends, and you can restart.

## Requirements

- Unity Game Engine
- C# (for scripting)
- Basic knowledge of Unity physics (Rigidbody2D, Colliders, etc.)

## Future Improvements

- Add difficulty scaling (increase pipe speed over time).
- Implement a main menu and settings screen.
- Introduce background music and more sound effects.
- Add character customization options.

Enjoy playing my simple game of Flappy Ghost! 👻
