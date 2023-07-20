# PYTHON-ASSIGNMENT-2
ASSIGNMENT GIVEN BY PROFF.CHENNA REDDY SIR
##########################################

Student details:-

1.N.Manogna - 22001A0510
2.T.Jyothirmayee - 22001A0504
3. G.V.Rishitha - 22001A\0509

**Cross the Road Game Documentation:**

**Overview:**
This code is a simple implementation of the "Cross the Road" game using the `turtle` module in Python. The player controls a character represented by a turtle, and the objective is to cross a busy road filled with moving cars. The player earns points by successfully crossing the road without colliding with any car. The game gets progressively more difficult as the player advances.

**Requirements:**
1. Python: This code requires Python to be installed on the system.
2. `turtle` module: The code uses the `turtle` module for graphics and user input.
3. The game runs on any operating system that supports Python and the `turtle` module.

**Game Elements:**
1. **Player (`player`):** Represents the player-controlled character.
2. **Car Manager (`car_manager`):** Manages the creation and movement of cars.
3. **Scoreboard (`scoreboard`):** Displays the player's score and level.

**Player Class (`player.py`):**
The `Player` class is responsible for creating and controlling the player character.

**Car Manager Class (`car_manager.py`):**
The `CarManager` class is responsible for creating and managing the cars' movement.

**Scoreboard Class (`scoreboard.py`):**
The `Scoreboard` class is responsible for displaying the player's score and level and handling game events such as game over and level up.

**Main Game Loop:**
The code runs an infinite loop (`while game_is_on:`) where the game progresses:
1. The screen updates with each iteration of the loop.
2. The player's character listens for keyboard inputs to control its movement.
3. New cars are created at regular intervals using the `car_manager.create_car()` method.
4. Existing cars move horizontally from left to right using the `car_manager.move_cars()` method.
5. The code checks for collisions between the player's character and any of the moving cars. If a collision is detected, the game ends, and the player receives a game over message.
6. The code checks if the player has successfully crossed the road. If the player reaches the finish line without colliding with any cars, the player's position is reset to the starting point (`player.go_to_start()`), and the game becomes more challenging (`car_manager.level_up()` and `scoreboard.increase_level()`).

**Scoring and Levels:**
- The player earns points by successfully crossing the road without colliding with any cars.
- The game has multiple levels, and as the player advances levels, the car speed and the number of cars increase, making the game more challenging.

**Usage:**
1. Ensure you have the required Python environment and modules installed.
2. Make sure the `player.py`, `car_manager.py`, and `scoreboard.py` files are present in the same directory as the main code.
3. Run the main code.
4. Use the "Up" arrow key to move the player's character upward and try to cross the road.
5. Avoid colliding with any cars.
6. The game will end if the player collides with a car, and the score and level will be displayed on the screen.
7. Close the game window by clicking on it.

**Note:**
- The game is designed to run indefinitely until the player chooses to close the game window manually.
