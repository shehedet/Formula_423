# 🏎️ FORMULA 423 🚴‍♂️

Welcome to our thrilling 2D racing game, built with Python and OpenGL! Race around an elliptical track, choosing between a nimble bike or a sturdy car, as you dodge obstacles, collect power-ups, and navigate the chaotic effects of banana pills that reverse your controls. With smooth physics, a dynamic HUD, and immersive first- or third-person views, this game challenges your reflexes and strategic skills to complete laps before time runs out. Ready to burn some virtual rubber? Dive in and take it for a spin!

## 🎮 Game Overview

In this high-speed racing adventure, your goal is to complete a set number of laps (`REQUIRED_LAPS`) on an elliptical track within a time limit (`TOTAL_TIME`). Choose your vehicle—bike or car—and tackle a track filled with cones, potholes, power-ups, power-downs, and banana pills. Avoid collisions that drain your health, grab power-ups to boost your speed, and brace for the control-reversing chaos of banana pills. The game features a sleek HUD displaying time, laps, speed, health, and active effects, making every race a pulse-pounding experience.

### Key Features
- **Two Vehicle Types**: Race as a bike (nimble, with leaning visuals) or a car (stable, with higher speed).
- **Dynamic Track**: Navigate an elliptical track with inner and outer boundaries, filled with randomly placed obstacles.
- **Obstacles**: Dodge cones and potholes that damage your vehicle upon collision.
- **Power-Ups & Power-Downs**:
  - **Power-Ups**: Boost your speed temporarily for a competitive edge.
  - **Power-Downs**: Reduce your remaining time, increasing the challenge.
  - **Banana Pills**: Reverse all controls (forward/backward, left/right) for 4 seconds, adding a wild twist.
- **Camera Modes**: Switch between first-person and third-person views for varied perspectives.
- **Health System**: Collisions reduce health; zero health ends the game.
- **Lap Tracking**: Complete laps by crossing the finish line, with angle-based detection for accuracy.
- **Responsive Physics**: Realistic acceleration, friction, and turning, adjusted for on-track and off-track conditions.
- **HUD**: Displays time remaining, laps completed, speed, health, and active power-up/banana pill effects.
- **Reset Option**: Restart the game at any time with the 'r' key.

## 🕹️ Controls

Master the controls to dominate the track:
- **Start Screen**:
  - `b`: Select bike and start the game.
  - `c`: Select car and start the game.
- **In-Game**:
  - `w`: Accelerate forward (reversed to backward when banana pill is active).
  - `s`: Accelerate backward (reversed to forward when banana pill is active).
  - `a`: Turn left (reversed to right when banana pill is active; bikes lean left).
  - `d`: Turn right (reversed to left when banana pill is active; bikes lean right).
  - `c`: Toggle between first-person and third-person camera modes.
  - `r`: Reset the game to the start screen.
  - `Esc`: Exit the game.
- **Note**: When a banana pill is active (orange circular objects), all controls reverse for 4 seconds, making 'w' move backward, 's' move forward, 'a' turn right, and 'd' turn left.

## 🛠️ Skills Showcased

This project demonstrates a range of technical and creative skills:
- **Game Development**: Designed a complete 2D racing game with core mechanics like movement, collision detection, and lap tracking.
- **Physics Simulation**: Implemented realistic vehicle dynamics, including acceleration, friction, and turning, with bike-specific leaning.
- **Graphics Programming**: Used OpenGL for rendering the track, vehicles, obstacles, power-ups, power-downs, and banana pills in 2D.
- **UI/UX Design**: Created an intuitive HUD to display critical game information (time, laps, speed, health, effects).
- **Object-Oriented Programming**: Structured the game using a `GameState` class to manage state and logic efficiently.
- **Randomized Level Design**: Developed algorithms to place obstacles and power-ups randomly while avoiding overlaps and ensuring fair placement.
- **Event Handling**: Managed keyboard inputs for responsive controls and game state changes.

## ⚡ Power-Ups and Banana Pills

Power-ups and banana pills add excitement and challenge to the gameplay:
- **Power-Ups** (`POWERUP_COUNT` blue objects):
  - **Effect**: Increase your maximum speed and current speed by a multiplier (`POWERUP_SPEED_MULTIPLIER`) for a duration (`POWERUP_DURATION`).
  - **Appearance**: Blue circular objects on the track.
  - **Strategy**: Grab these to overtake opponents or recover from off-track slowdowns.
- **Power-Downs** (`POWERDOWN_COUNT` red objects):
  - **Effect**: Reduce remaining time by a set amount (`POWERDOWN_TIME_REDUCTION`), risking a game over if time runs out.
  - **Appearance**: Red circular objects on the track.
  - **Strategy**: Avoid these to maintain your time buffer and stay in the race.
- **Banana Pills** (`BANANA_PILL_COUNT` orange objects):
  - **Effect**: Reverse all controls for 4 seconds (`BANANA_PILL_DURATION`): 'w' moves backward, 's' moves forward, 'a' turns right, 'd' turns left (bikes lean oppositely).
  - **Appearance**: Orange circular objects on the track.
  - **Strategy**: Prepare for sudden control changes; use strategically to disrupt opponents in multiplayer (if implemented).

## 🌟 Additional Features
- **Track Design**: Elliptical track with inner and outer boundaries, defined by configurable radii (`TRACK_INNER_X_RADIUS`, `TRACK_OUTER_X_RADIUS`, etc.).
- **Obstacle Placement**: Cones, potholes, power-ups, power-downs, and banana pills are placed randomly with collision checks to prevent overlap and ensure fair distribution.
- **Health and Respawn**: Collisions reduce health (`HEALTH_DECREMENT`); off-track or boundary collisions trigger a respawn with a flicker effect (`RESPAWN_DELAY`).
- **Camera Dynamics**: Adjustable camera distance and height, with smooth transitions between first- and third-person modes.
- **Game Over Conditions**: End the game if time runs out, health reaches zero, or required laps are completed, displaying final time.
- **Reset Functionality**: Fully resets game state, including player position, obstacles, power-ups, and banana pills, for a fresh start.

## 💻 Languages and Libraries Used
- **Languages**:
  - **Python**: Core language for game logic, physics, and rendering.
- **Libraries**:
  - **PyOpenGL**: For 2D rendering of the track, vehicles, obstacles, and effects.
  - **PyOpenGL-accelerate**: Performance optimization for OpenGL bindings.
  - **GLUT (OpenGL Utility Toolkit)**: Handles window creation, input handling, and display callbacks.
  - **math**: For trigonometric calculations in track design, movement, and collision detection.
  - **random**: For randomized placement of obstacles, power-ups, power-downs, and banana pills.
  - **time**: For timing game events, lap tracking, and effect durations.

## 📧 About Us
- [akm.shahadat.hossain@g.bracu.ac.bd](mailto:akm.shahadat.hossain@g.bracu.ac.bd)
- [eftekhar.tanvir.efti@g.bracu.ac.bd](mailto:eftekhar.tanvir.efti@g.bracu.ac.bd)
- [syed.izdian.siraji@g.bracu.ac.bd](mailto:syed.izdian.siraji@g.bracu.ac.bd)
