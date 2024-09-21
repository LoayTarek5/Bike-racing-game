# Rising Sun Bike Racing Game

This is a 2D bike racing game developed using SDL (Simple DirectMedia Layer) in C++. The game features a bike that can jump over obstacles and navigate through a scrolling background.

## Project Structure

The project consists of several key files:

- `main.cpp`: The entry point of the application.
- `constants.h`: Defines various constants used throughout the game.
- `coardinate.h`: Contains classes for handling coordinates and game objects.
- `collision.h`: Implements collision detection logic.
- `function.h`: Defines utility functions like `apply_surface` for rendering.
- `menu.h`: Implements the game's menu system.
- `process.h`: Contains the main game loop and mechanics.
- `variable.h`: Declares global variables used across the game.
- `init.h`: Contains initialization code and resource loading functions.
- `bike race.cbp`: CodeBlocks project file.
- `bike race.depend`: Dependency file for the project.
- `bike race.layout`: CodeBlocks layout file.

## Dependencies

The game relies on the following libraries:

- SDL (Simple DirectMedia Layer)
- SDL_image
- SDL_ttf

Ensure these libraries are installed on your system before attempting to build the project.

## Building the Project

This project uses CodeBlocks as its IDE. To build the project:

1. Open the `bike race.cbp` file in CodeBlocks.
2. Ensure all necessary libraries (SDL, SDL_image, SDL_ttf) are properly linked.
3. Build the project using the CodeBlocks build command.

## Project Setup

1. The game initializes SDL and its subsystems (Video, Event Handling, File I/O, and Threading).
2. The video mode is set to 800x600 pixels with 32-bit color depth.
3. TTF (TrueType Font) is initialized for text rendering.
4. Various image resources are loaded, including backgrounds, bike sprite, and obstacles.
5. Font files are loaded for text rendering.

## Game Features

- The game window is titled "RISING SUN BIKE RACING GAME".
- The bike starts at x-coordinate 150 and can move up to x-coordinate 250.
- The game includes a scrolling background and two types of obstacles (walls).
- The bike can jump using the spacebar or up arrow key.
- Collision detection is implemented for obstacles.
- A timer displays the elapsed time during gameplay, with a time limit of 1:30 minutes.
- The game features a menu system with options to play, view instructions, or quit.

## Game Controls

- Right Arrow: Increase speed
- Left Arrow: Decrease speed
- Spacebar / Up Arrow: Jump
- Escape: Exit the game

## Resource Files

The game requires the following resource files in the `image` folder:
- `bg1.png`, `bg2.png`: Background images
- `bike.PNG`: Bike sprite
- `wall.JPG`, `wall1.JPG`: Obstacle images
- `menu.jpg`, `menu_play.jpg`, `menu_instruction.jpg`, `menu_exit.jpg`: Menu images

Additionally, a `times.ttf` font file is required for text rendering.

## Code Overview

- `init.h`: Handles SDL initialization, window creation, and resource loading.
- `function.h`: Defines the `apply_surface` function for rendering images to the screen.
- `menu.h`: Implements the start menu with options for play, instructions, and quit.
- `process.h`: Contains the `bike_process` class, which handles the main game loop, including bike movement, jumping mechanics, and obstacle management.
- `variable.h`: Declares global variables for surfaces, fonts, game states, and other necessary elements.

## Game Mechanics

- The bike's vertical position is controlled by a jumping mechanism.
- The game speed increases or decreases based on user input.
- The background and obstacles scroll to create the illusion of movement.
- Collisions with obstacles end the game.
- The game ends when the player reaches the time limit or collides with an obstacle.

## Note for Developers

This project is a work in progress. Ensure all necessary files are present and properly linked before attempting to build and run the game. If you encounter any issues with resource loading, check that all image and font files are in the correct locations relative to the executable.
