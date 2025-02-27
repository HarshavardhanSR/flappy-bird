# FLAPPY BIRD
Flappy bird flew into an endless pipe zone (or is it?) and needs help flying through to get out.  

# ABOUT THE GAME
A simple side-scrolling game where the player controls a bird to fly between pipes without hitting them.  Flying between each set of pipes scores 1 point and hitting them or the ground ends the game.  See how long you can last and set records.  


## 🔧 How to Run  
1. Clone this repository:  
   ```sh
   git clone https://github.com/HarshavardhanSR/flappy-bird.git
2. Open index.html in a browser.
2. Start playing! 🚀




# TECHNOLOGY
 * HTML/CSS on canvas
 * JavaScript for game logic

# MVP
 * start the game with a 'press button'
 * bird falls default to gravity
 * bird flies to 'click' (might be better for mobile capabilities)
 * pipes spawn top and bottom and scroll to the left 
 * track score
 * end game on collision

# STRETCH GOALS
 * animate bird
 * add sounds for scoring, flying, and collision
 * a customized theme
 * game is animated while waiting for player to start game
 * night time / day time
 * add a running time to display
 * make the game web responsive

# GAMEPLAN
---
## HTML
 - [X] container for gaming screen
 - [X] game title
 - [X] game screen `<canvas>`

## CSS
 - [X] *centered* game title
 - [X] *centered* game screen

## JavaScript
### Pieces I need
 - [X] specify canvas size
 - [X] draw bird image
 - [X] top pipe image
 - [X] constant gap between pipes
 - [X] bottom pipe image
 - [X] score tracker
 - [X] ready screen: game state 0
 - [X] game over screen: game state 2
 - [X] background image
 - [X] ground image
 - [X] sounds on flying, collision, scoring, falling, and game over screen
### Functions I need
 - [X] start game: game state 1
    - [X] start on 'click' (mobile compatible)
    - [X] spawn set of pipes with constant gap
      - [X] if statement triggering at x-coordinate
 - [X] bird's movement
    - [X] gravity: bird's y-coordinate increases to fall  
     * velocity's value is incremented by gravity constant
     * bird's position function updates velocity's value
    - [X] flying: bird's y-coordinate decreases to fly on 'click'
        - [X] eventListener 'click' (also enabled 'spacebar')
    - [X] rotate bird upward each time it flies (smells like a challenge)
        - [X] animation object / array of images to flip through
 - [X] a drawing function to animate game
   - [X] place images and loop
    - [X] pipes' x-coordinates decrease to scroll left
        - [X] increment score by 1 upon passing pipe
    - [X] pipes' y-coordinates are generated randomly
    - [X] draw background
    - [X] draw bird
 - [X] Game Over: game state 2
    - [X] collision with pipes
    - [X] collision with floor and canvas ceiling
    - [X] cut screen
    - [X] restart game on 'click' start button
        - [ ] display best score
        - [X] display current score
        - [X] reset score on start game
        - [X] reset pipes
 

> Infinite pipe spawning has been a road block for me.  Animating canvas images seem even more challenging.

> Tracking the score was challenging due to the fact that each place value of the number had to correlate to an image of its value. No texts and fonts were used in the game.

> Overall, I learned a lot of canvas tools and mechanics for JavaScript.  Re-creating this game was a lot of fun and good training for various JavaScript fundamentals such as loops, functions, if-else statements, arrays, objects, and concepts.
