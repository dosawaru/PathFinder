# Project Title: Path Finding Algorithm Visualization

## Motivation
This project aims to visualize the process of finding the shortest path between two points on a grid using the A* algorithm. Pathfinding algorithms are widely used in computer science, robotics, and gaming to find the most efficient route from one location to another. This project provides an interactive tool to explore and understand how the A* algorithm works in a grid-based environment.


## Demo

### Basic Example

![2023-10-13 19-52-19](https://github.com/dosawaru/PathFinder/assets/35234154/ff305d18-772e-473f-a21a-35ba508b58ce)

![Screenshot 2023-10-13 19-52-53](https://github.com/dosawaru/PathFinder/assets/35234154/4ae5a1aa-fc80-453c-bda1-8b31e3bbe6c9)

### Simple Example

![2023-10-13 19-54-14](https://github.com/dosawaru/PathFinder/assets/35234154/ed9dd32c-78ae-4117-9031-52e9da823af7)

![Screenshot 2023-10-13 19-54-42](https://github.com/dosawaru/PathFinder/assets/35234154/f47ac461-8a54-482c-837a-92b356018ba0)

### Complex Example

![2023-10-13 19-56-49](https://github.com/dosawaru/PathFinder/assets/35234154/2d69cd97-5af2-41fc-b906-babaaa3a4504)

![Screenshot 2023-10-13 19-57-40](https://github.com/dosawaru/PathFinder/assets/35234154/a5c65404-6f48-4085-b38e-8ffcac422320)


## Installation
1. Make sure you have Python installed on your system.
2. Clone or download this repository to your local machine.
3. Install the required libraries using pip:
   ```
   pip install pygame
   ```
   
## Usage
1. Run the script `main.py` to launch the pathfinding algorithm visualization.
2. Follow the on-screen instructions:
   - Left-click to place the start and end nodes.
   - Left-click on the grid to add barrier nodes.
   - Right-click to remove nodes.
   - Press the space bar to start the pathfinding algorithm.
   - Press 'C' to clear the grid.
   - Press 'Q' to exit the application.

## Functions
- `Node`: Represents individual squares on the grid with various attributes and methods to manage their properties.

- `h(p1, p2)`: Computes the Manhattan distance between two points, used as the heuristic function in the A* algorithm.

- `draw_path(came_from, current, draw)`: Draws the shortest path on the grid based on the "came_from" dictionary.

- `algorithm(draw, grid, start, end)`: Implements the A* algorithm to find the shortest path from the start to the end node.

- `create_grid(rows, width)`: Creates the grid by initializing a 2D array of Node objects.

- `draw_grid(win, rows, width)`: Draws the grid lines on the screen.

- `draw(win, grid, rows, width)`: Draws the entire grid on the screen.

- `get_position(pos, rows, width)`: Converts mouse coordinates to grid row and column.

- `main(win, width)`: Main function to manage user interactions, start the application, and handle input events.

## Libraries
The project uses the following libraries:
- `pygame`: Used for creating the graphical user interface and managing user interactions.
- `Tkinter`: Used for displaying information messages and confirmation dialogs.

Feel free to explore and experiment with the pathfinding algorithm visualization tool. It can help you understand how the A* algorithm works and how paths are computed in grid-based environments.
