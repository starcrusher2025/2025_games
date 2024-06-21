```markdown
# Game Engine Package - starcrusher2025

## Introduction
This package provides a simple game engine framework named starcrusher2025. It allows developers to create 2D games using Pygame by providing essential functionalities such as managing the game window, controlling player entities, handling input, and rendering.

## Installation
To install starcrusher2025-games, use pip:

```bash
pip install starcrusher2025-games
```

## Usage
To use starcrusher2025 in your Python projects, follow the examples below:

```python
from starcrusher2025_games import Game

# Initialize the game instance
game = Game()

# Set the background color of the game window
game.window.set_bgc(0, 0, 0)  # Sets the background to black

# Set player attributes
game.player.set_color(255, 0, 0)  # Sets the player color to red
game.player.set_start_pos((400, 300))  # Sets the player starting position
game.player.set_size((50, 50))  # Sets the player size
game.player.set_speed(5)  # Sets the player speed
game.player.load_image("player.png")  # Loads an image for the player
game.set_fps(60) #Sets the fps on 60

# Set window size
game.window.set_size(800, 600)  # Sets the game window size

# Start the game loop
game.start()
```

## Commands

### `game.window.set_bgc(r, g, b)`
Sets the background color of the game window.

- **Parameters:**
  - `r`: Integer representing the red component of the RGB color (0-255).
  - `g`: Integer representing the green component of the RGB color (0-255).
  - `b`: Integer representing the blue component of the RGB color (0-255).

### `game.player.set_start_pos(start_pos)`
Sets the starting position of the player entity.

- **Parameters:**
  - `start_pos`: Tuple representing the `(x, y)` coordinates of the starting position.

### `game.player.set_size(size)`
Sets the size of the player entity.

- **Parameters:**
  - `size`: Tuple representing the `(width, height)` of the player entity.

### `game.player.set_speed(speed)`
Sets the speed of the player entity.

- **Parameters:**
  - `speed`: Integer value representing the speed of the player.

### `game.player.get_player_position()`
returns the player position

### `game.player.load_image(image_path)`
Loads an image file for the player entity.

- **Parameters:**
  - `image_path`: Path to the image file to be loaded for the player.

### `game.window.set_size(width, height)`
Sets the size of the game window.

- **Parameters:**
  - `width`: Width of the game window in pixels.
  - `height`: Height of the game window in pixels.

### `game.window.set_bgc(r,g,b)`
Sets the background color of the game window.

- **Parameters:**
  - `color`: Tuple representing the RGB color values (e.g., `(0, 0, 0)` for black).

### `game.start()`
Starts the game loop, which handles game logic, rendering, and input handling until the game is stopped or closed.

### `game.stop()`
Stops the game loop and terminates the game.
