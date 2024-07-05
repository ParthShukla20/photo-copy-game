## Set-Up the project.

1) Clone the repository (https://github.com/ParthShukla20/photo-copy-game.git)
2) open project and install node modules (npm install)
3) To launch the Project execute command "node server.js"

## Code Structure and Design Decisions

The repository is structured into two main components:

# 1) Server Component: server.js

  This file serves as the backend of the project.
  It utilizes Node.js for the runtime environment, Express.js for server setup, and Socket.io for real-time communication.

# 2) Public Directory: public

  This directory contains the client-side files necessary for the game.
  
  # It includes three main files:
  
  index.html: Dedicated to the game UI.
  home.html: Acts as the landing page and includes a form for players to enter their names.
  game.js: Contains the game logic, including functions for deciding the winner, managing the timer, handling shapes, and maintaining the pattern area.
 
## Server.js

  Sets up the Express server.
  Manages socket connections for real-time communication between players.
  Handles the routing for serving the HTML files.

# public/home.html

The landing page of the game.
Includes a form for players to input their names before starting the game.

# public/index.html

  The main game interface.
  Displays the circular pattern area and various shapes (quarter-circle, half-circle, three-quarter-circle) in colors yellow, purple, and blue.
  Contains the game UI elements like timers and pattern areas.

# public/game.js

  Implements the game logic using modular and functional programming.
  Contains separate functions for different tasks and components such as:
  determineRoundWinner(): Determines the winner of the game.
  startTimer(): Manages the game timer.
  placeShape(): Handles the creation and display of shapes.
  updatePatternArea(): Maintains and updates the pattern area.
  
# How to Play

  Open the home.html page in a web browser.
  Enter your player name in the form and submit.
  The game will redirect to index.html, where the game UI is displayed.
  Follow the game instructions to replicate the given patterns using the provided shapes within the time limit.
  The game determines the winner based on the winner of alteast 2 rounds in total of 3 rounds .
