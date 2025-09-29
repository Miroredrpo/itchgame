# Platformer Dash

A fast-paced geometric platformer game built with p5.js where you control a rotating cube through an obstacle course.

## How to Play

1. Open `index.html` in your browser to start at the main menu
2. Click "Play Now" to begin the game
3. Use the following controls:
   - Press `SPACE` or `UP ARROW` to jump
   - Press `R` to restart after game over
   
## Features

- Auto-scrolling platformer gameplay 
- Physics-based movement with momentum and rotation
- Obstacles:
  - Black platforms to jump on
  - Black triangular spikes to avoid
- Game over screen when hitting spikes or falling off screen
- Camera that follows player's vertical movement

## Technical Details

Built using:
- [p5.js](https://p5js.org/) for graphics and game loop
- HTML5 Canvas for rendering
- CSS for styling and layout

## Level Design

The level is built using an array of objects:
- `blo` - Platform blocks for landing
- `spi` - Spike obstacles that cause death on contact

## Files

- `index.html` - Main menu
- `game.html` - Game container
- `mySketch.js` - Game logic and rendering

## Development

To modify the level layout, edit the `lCode` array in `mySketch.js`. Level objects are defined as:

```js
["type", x, y]
```

Where:
- `type` is either "blo" (block) or "spi" (spike)
- `x` and `y` are grid coordinates (multiples of 40)
