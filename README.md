# Flappy-bird
Flappy Bird game project built using vanilla HTML, CSS, and JavaScript 
# About the Game
A simple side-scrolling game where the player controls a bird to fly between pipes without hitting them. Flying between each set of pipes scores 1 point and hitting them or the ground ends the game. See how long you can last and set records.

## 🔧 How to Run  
1. Clone this repository:  
   ```sh
   git clone https://github.com/HarshavardhanSR/flappy-bird.git
2. Open index.html in a browser.
3. Start playing! 🚀

# MVP
1) start the game with a 'press button'
2) bird falls default to gravity
3) bird flies to 'click' (might be better for mobile capabilities)
4) pipes spawn top and bottom and scroll to the left
5) track score
6) end game on collision
# STRETCH GOALS
1. animate bird
2. add sounds for scoring, flying, and collision
3. a customized theme
4. game is animated while waiting for player to start game
5. night time / day time
6. add a running time to display
7. make the game web responsive
# GAMEPLAN
# HTML
1. container for gaming screen
2. game title
3. game screen <canvas>
# CSS
1. centered game title
2. centered game screen
# Pieces You Need
1. Canvas Setup – Specify canvas size.
2. Bird Image – Draw bird sprite.
3. Top Pipe Image – Load and draw the top pipe.
4. Pipe Gap – Maintain a constant gap between pipes.
5. Bottom Pipe Image – Load and draw the bottom pipe.
6. Score Tracker – Track and display the score.
7. Ready Screen – Display when the game state is 0 (before starting).
8. Game Over Screen – Display when the game state is 2.
9. Background Image – Load and draw the background.
10. Ground Image – Load and draw the ground.
11. Sounds – Add sound effects for:
        1. Flying
        2. Collision
        3. Scoring
        4. Falling
        5. Game Over

# Functions You Need Start Game (startGame()) – Change game state to 1.
1. Start on Click (handleClick()) – Trigger game start on mobile tap or spacebar.
2. Spawn Pipes (spawnPipes()) – Generate pipes with a constant gap.
3. Pipe Movement (movePipes()) – Shift pipes left across the screen.
4. Pipe Collision Check (checkPipeCollision()) – Detect if the bird hits pipes.
5. Bird Movement (updateBird()) – Adjust bird’s position with gravity.
6. Gravity (applyGravity()) – Increase bird’s downward velocity over time.
7. Flying (fly()) – Move bird upward when clicking or pressing space.
8. Bird Rotation (rotateBird()) – Rotate the bird upward when flying.
9. Bird Animation (animateBird()) – Flip through images for animation.
10. Draw Game (drawGame()) – Render all elements continuously.
11. Score Update (updateScore()) – Increment score when passing a pipe.
12. Pipe Randomization (randomPipeY()) – Randomly generate pipe heights.
13. Draw Background (drawBackground()) – Render the background image.
14. Draw Bird (drawBird()) – Render the bird sprite.
15. Game Over (gameOver()) – Trigger game over (state 2) on collision.
16. Collision Check (checkCollision()) – Detect collision with pipes, floor, or ceiling.
17. Cut Screen (cutScreen()) – Display game over overlay.
18. Restart Game (restartGame()) – Reset game on click.
19. Display Best Score (displayBestScore()) – Show the highest score.
20. Display Current Score (displayScore()) – Show current score.
21. Reset Score (resetScore()) – Set score back to 0 on restart.
22. Reset Pipes (resetPipes()) – Clear pipes when restarting the game.
