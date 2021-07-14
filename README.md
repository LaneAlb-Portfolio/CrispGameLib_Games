<a href="https://abagames.github.io/crisp-game-lib-games/?survivor"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/survivor/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?chargebeam"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/chargebeam/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?pillars3d"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/pillars3d/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?slalom"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/slalom/screenshot.gif" width="25%" loading="lazy"></a>

<h1 align="center">crisp-game-lib</h1>

<a href="https://abagames.github.io/crisp-game-lib-games/?doshin"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/doshin/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?cardq"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/cardq/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?earock"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/earock/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?shiny"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/shiny/screenshot.gif" width="25%" loading="lazy"></a>

`crisp-game-lib` is a JavaScript library for creating browser games quickly and easily. I developed [50 minigames in 2014](http://www.asahi-net.or.jp/~cs8k-cyu/blog/2014/12/12/games-in-2014/), as well as the Haxe library [mgl](https://github.com/abagames/mgl) and the CoffeeScript library [mgl.coffee](https://github.com/abagames/mgl.coffee) to make them. After that I continued to work on minigames and libraries. Using this experience, `crisp-game-lib` was created as a library with the minimum functionality necessary to create classic arcade-like minigames.

The `crisp-game-lib` itself is well dogfooded, and I have already created [more than 100 games](https://github.com/abagames/crisp-game-lib#demo-click-the-image-to-play) in a short time using this library. By simply writing a single JavaScript file with the game `title`, `description`, and an `update` function that is called 60 times per second, you can create a browser game that runs on PC and mobile devices. The functions necessary for the mini-game are provided in the form of [functions for drawing](https://github.com/abagames/crisp-game-lib#drawing-demo) boxes, lines, arcs, text, characters, [a collision detection function](https://github.com/abagames/crisp-game-lib#collision-demo) integrated with these drawing functions, [an input acquisition function](https://github.com/abagames/crisp-game-lib#input-demo) that supports both mouse and touch panel, and [a sound effect function](https://github.com/abagames/crisp-game-lib#sound-demo) that allows the developer to simply select the name of the sound to be played. In addition, there are functions to make the game juicy, such as background music that is automatically generated by setting `isPlayingBgm` to true as [an option](https://github.com/abagames/crisp-game-lib#options), replay function that is enabled by setting `isReplayEnabled` to true, the ability to change the appearance of the game to retro CRT style or dot picture style by simply setting `theme`, and pixel arts that can be easily defined with the `characters` array.

It also has [type definitions in TypeScript](https://github.com/abagames/crisp-game-lib/blob/master/docs/bundle.d.ts), so you can fully benefit from IntelliSense on [VSCode](https://code.visualstudio.com/). Please refer to [the sample code](https://github.com/abagames/crisp-game-lib#sample-code) and [reference](https://github.com/abagames/crisp-game-lib#reference) below for more details on what kind of code you should write.

See also [the article about crisp-game-lib](https://terrysfreegameoftheweek.com/kento-chos-crisp-game-lib-games/) written by [Terry Cavanagh](https://twitter.com/terrycavanagh), known as the developer of [Super Hexagon](https://store.steampowered.com/app/221640/Super_Hexagon/) and [VVVVVV](https://store.steampowered.com/app/70300/VVVVVV/). A list of the browser games I've made can be found on [my web page](http://www.asahi-net.or.jp/~cs8k-cyu/browser.html). By looking at the gif animations of each game, you can easily understand its rules.

## Demo (Click the image to play)

<a href="https://abagames.github.io/crisp-game-lib-games/?cywall"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/cywall/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?lland"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/lland/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?bamboo"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/bamboo/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?subjump"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/subjump/screenshot.gif" width="25%" loading="lazy"></a>

<a href="https://abagames.github.io/crisp-game-lib-games/?grenadier"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/grenadier/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?catep"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/catep/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?zoneb"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/zoneb/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?laserfortress"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/laserfortress/screenshot.gif" width="25%" loading="lazy"></a>

<a href="https://abagames.github.io/crisp-game-lib-games/?pressm"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/pressm/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?rebirth"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/rebirth/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?numberball"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/numberball/screenshot.gif" width="25%" loading="lazy"></a><a href="https://abagames.github.io/crisp-game-lib-games/?arcfire"><img src="https://github.com/abagames/crisp-game-lib-games/raw/main/docs/arcfire/screenshot.gif" width="25%" loading="lazy"></a>

Other games are listed on [my browser games page](http://www.asahi-net.or.jp/~cs8k-cyu/browser.html).

## Sample code

[![pinclimb screenshot](https://github.com/abagames/crisp-game-lib-games/raw/main/docs/pinclimb/screenshot.gif)](https://abagames.github.io/crisp-game-lib-games/?pinclimb)

```javascript
// Write the game name to 'title'.
title = "PIN CLIMB";

// 'description' is displayed on the title screen.
description = `
[Hold] Stretch
`;

// User-defined characters can be written here.
characters = [];

// Configure game options.
options = {
  isPlayingBgm: true,
  isReplayEnabled: true,
  // If you want to play a different BGM or SE,
  // you can try changing the 'seed' value used to generate sounds.
  seed: 400,
};

// (Optional) Defining the types of variables is useful for
// code completion and error detection.
/** @type {{angle: number, length: number, pin: Vector}} */
let cord;
/** @type {Vector[]} */
let pins;
let nextPinDist;
const cordLength = 7;

// 'update()' is called every frame (60 times per second).
function update() {
  // 'ticks' counts the number of frames from the start of the game.
  if (!ticks) {
    // Initialize the game state here. (ticks === 0)
    pins = [vec(50, 0)]; // 'vec()' creates a 2d vector instance.
    nextPinDist = 10;
    cord = { angle: 0, length: cordLength, pin: pins[0] };
  }
  // 'difficulty' represents the difficulty of the game.
  // The value of this variable is 1 at the beginning of the game and
  // increases by 1 every minute.
  let scr = difficulty * 0.02;
  if (cord.pin.y < 80) {
    scr += (80 - cord.pin.y) * 0.1;
  }
  // 'input.isJustPressed' is set to true the moment the button is pressed.
  if (input.isJustPressed) {
    // 'play()' plays the SE.
    play("select");
  }
  // 'input.isPressed' is set to true while the button is pressed.
  if (input.isPressed) {
    cord.length += difficulty;
  } else {
    cord.length += (cordLength - cord.length) * 0.1;
  }
  cord.angle += difficulty * 0.05;
  // Draw a line connecting the coordinates of
  // the first argument and the second argument.
  line(cord.pin, vec(cord.pin).addWithAngle(cord.angle, cord.length));
  if (cord.pin.y > 98) {
    play("explosion");
    // Call 'end()' to end the game. (Game Over)
    end();
  }
  let nextPin;
  // 'remove()' passes the elements of the array of the first argument to
  // the function of the second argument in order and executes it.
  // If the function returns true, the element will be removed from the array.
  remove(pins, (p) => {
    p.y += scr;
    // Draw a box and check if it collides with other black rectangles or lines.
    if (box(p, 3).isColliding.rect.black && p !== cord.pin) {
      nextPin = p;
    }
    return p.y > 102;
  });
  if (nextPin != null) {
    play("powerUp");
    // Add up the score.
    // By specifying the coordinates as the second argument,
    // the added score is displayed on the screen.
    addScore(ceil(cord.pin.distanceTo(nextPin)), nextPin);
    cord.pin = nextPin;
    cord.length = cordLength;
  }
  nextPinDist -= scr;
  while (nextPinDist < 0) {
    // 'rnd()' returns a random value.
    pins.push(vec(rnd(10, 90), -2 - nextPinDist));
    nextPinDist += rnd(5, 15);
  }
}
```

## More sample codes

Sample code for each game is `main.js` in each directory in the [docs directory](https://github.com/abagames/crisp-game-lib-games/tree/main/docs).

## Getting started

1. Download [docs/getting_started/index.html](https://github.com/abagames/crisp-game-lib/blob/master/docs/getting_started/index.html).

1. Open `index.html` in a text editor and write the code of your game in the `<script>` element.

1. Open `index.html` in a browser and play the game.

1. You can publish the game by putting `index.html` on your web server.

## Write your own game (with the help of IntelliSense and Live Reload)

1. Clone or [download](https://github.com/abagames/crisp-game-lib/archive/refs/heads/master.zip) this repository.

1. `npm install`

1. Copy the `docs/_template` directory and rename it to `[your own game name]`.

1. Open `docs/[your own game name]/main.js` with the editor ([VSCode](https://code.visualstudio.com/) is recommended) and write your own game code.

1. `npm run watch_games`

1. Open the URL `http://localhost:4000?[your own game name]` with a browser. The page is live-reloaded when the code is rewritten.

## Publish your own game

1. Place `main.js`, [docs/bundle.js](https://github.com/abagames/crisp-game-lib/blob/master/docs/bundle.js) and [docs/index.html](https://github.com/abagames/crisp-game-lib/blob/master/docs/index.html) on the web server in the following directory structure.

   ```
   ┝ [games root directory (any name)]
      ┝ [your own game name]
      │  └ main.js
      ┝ bundle.js
      └ index.html
   ```

1. Open the URL `[Address of games root directory]/index.html?[your own game name]` with a browser.

## Reference

### Drawing ([DEMO](https://abagames.github.io/crisp-game-lib-games/?ref_drawing))

[![ref_drawing screenshot](https://github.com/abagames/crisp-game-lib-games/raw/main/docs/ref_drawing/screenshot.gif)](https://abagames.github.io/crisp-game-lib-games/?ref_drawing)

```javascript
function update() {
  // Set the drawing color.
  // color(colorName : "transparent" | "white" |
  // "black" | "red" | "green" | "blue" |
  // "yellow" | "purple" | "cyan" |
  // "light_black" | "light_red" | "light_green" | "light_blue" |
  // "light_yellow" | "light_purple" | "light_cyan");
  color("red");
  // Draw the box.
  // box(x, y, width, height?);
  // box(pos, size);
  box(20, 20, 15, 20);
  // Draw the rectangle.
  // rect(x, y, width, height?);
  // rect(pos, size);
  rect(70, 20, 20, 25);
  // Draw the bar.
  // bar(x, y, length, thickness, rotate, centerPosRatio?);
  // bar(pos, length, thickness, rotate, centerPosRatio?);
  bar(20, 70, 18, 5, 0.7, 0.5);
  // Draw the line.
  // line(x1, y1, x2, y2, thickness);
  // line(p1, p2, thickness);
  line(70, 70, 90, 80);
  // Draw the arc.
  // arc(x, y, radius, thickness?, angleFrom?, angleTo?);
  // arc(pos, radius, thickness?, angleFrom?, angleTo?);
  arc(30, 60, 20, 5, 0.1, 1.5);
  // Draw the text.
  // text(string, x, y, options?);
  // text(string, p, options?);
  text("a", 10, 20);
  // Draw the user defined character.
  // char(string, x, y, options?);
  // char(string, p, options?);
  char("a", 30, 40);
}
```

Setting the color prior to `char()` will recolor the sprite. Use `color("black")` to restore and use the original colors.

```javascript
// Recolor the sprite entirely to blue
color("blue");
char("a", 10, 10);

// Draw the character with original specified colors from the characters array
color("black");
char("a", 10, 10);
```

### Collision ([DEMO](https://abagames.github.io/crisp-game-lib-games/?ref_collision))

[![ref_collision screenshot](https://github.com/abagames/crisp-game-lib-games/raw/main/docs/ref_collision/screenshot.gif)](https://abagames.github.io/crisp-game-lib-games/?ref_collision)

```javascript
function update() {
  color("purple");
  box(50, 50, 20, 10);
  color("green");
  // Check if the drawn figure collides a rect/text/char.
  // [Drawing function].isColliding => {
  //   rect.[color]: boolean;
  //   text.[char]: boolean;
  //   char.[char]: boolean;
  // }
  // If the drawing box collides the purple rect...
  if (box(input.pos, 5, 5).isColliding.rect.purple) {
    end();
  }
}
```

The graphics must be drawn prior to handling the collision. As such, to establish a two-way interaction between two types of objects (e.g. both the bullet and the target are destroyed upon colliding), at least one must have its graphic representation drawn independently first. As an example, the following block is an excerpt from [the game `S LANES`](https://abagames.github.io/crisp-game-lib-games/?slanes) with comments added:

```javascript
shots.forEach((s) => {
  // Updates for bullets

  // Drawing of graphic representation/hitbox for bullets
  char("d", s.pos);
});

remove(enemies, (e) => {
  // Updates for enemies

  // Handling collision with bullets from enemies
  // This conditional statement also draws onscreen graphics
  if (char("b", e.pos).isColliding.char.d) {
    play("powerUp");
    particle(e.pos);
    coins.push({ pos: e.pos, laneIndex: e.laneIndex });
    return true;
  }
});

remove(shots, (s) => {
  // Handling collision with enemies from bullets
  return s.pos.x > 103 || char("d", s.pos).isColliding.char.b;
});
```

Also see: notes about the `remove()` function from the sample code of `PIN CLIMB` above.

### Input ([DEMO](https://abagames.github.io/crisp-game-lib-games/?ref_input))

```javascript
function update() {
  // 'input' variable returns the input status.
  // input => {
  //   pos: Vector;
  //   isPressed: boolean;
  //   isJustPressed: boolean;
  //   isJustReleased: boolean;
  // }
  color(input.isPressed ? "red" : "blue");
  box(input.pos, 10, 10);
}
```

### Sound ([DEMO](https://abagames.github.io/crisp-game-lib-games/?ref_sound))

```javascript
function update() {
  // Plays a sound effect.
  // play(type: "coin" | "laser" | "explosion" | "powerUp" |
  // "hit" | "jump" | "select" | "lucky");
  play("coin");
}
```

### Other variables and functions

```typescript
// Game ticks (60 ticks = 1 second)
let ticks: number;
// Game difficulty (starts at 1, incremented by 1 per minute)
let difficulty: number;
// Game score
let score: number;

// Add up score.
function addScore(value: number);
function addScore(value: number, x: number, y: number);
function addScore(value: number, pos: VectorLike);

// Add particles.
function particle(
  x: number,
  y: number,
  count?: number,
  speed?: number,
  angle?: number,
  angleWidth?: number
);
function particle(
  pos: VectorLike,
  count?: number,
  speed?: number,
  angle?: number,
  angleWidth?: number
);

// End game. (Game Over)
function end(): void;

// Return random number.
function rnd(lowOrHigh?: number, high?: number);
// Return random integer.
function rndi(lowOrHigh?: number, high?: number);
// Return positive or negative random number.
function rnds(lowOrHigh?: number, high?: number);

// Return Vector instance.
function vec(x?: number | VectorLike, y?: number): Vector;

class Vector {
  x: number;
  y: number;
  constructor(x?: number | VectorLike, y?: number);
  set(x?: number | VectorLike, y?: number): this;
  add(x?: number | VectorLike, y?: number): this;
  sub(x?: number | VectorLike, y?: number): this;
  mul(v: number): this;
  div(v: number): this;
  clamp(xLow: number, xHigh: number, yLow: number, yHigh: number): this;
  wrap(xLow: number, xHigh: number, yLow: number, yHigh: number): this;
  addWithAngle(angle: number, length: number): this;
  swapXy(): this;
  normalize(): this;
  rotate(angle: number): this;
  angleTo(x?: number | VectorLike, y?: number): number;
  distanceTo(x?: number | VectorLike, y?: number): number;
  isInRect(x: number, y: number, width: number, height: number): boolean;
  equals(other: VectorLike): boolean;
  floor(): this;
  round(): this;
  ceil(): this;
  length: number;
  angle: number;
}

interface VectorLike {
  x: number;
  y: number;
}

const PI: number;
function abs(v: number): number;
function sin(v: number): number;
function cos(v: number): number;
function atan2(y: number, x: number): number;
function pow(b: number, e: number): number;
function sqrt(v: number): number;
function floor(v: number): number;
function round(v: number): number;
function ceil(v: number): number;
function clamp(v: number, low?: number, high?: number): number;
function wrap(v: number, low: number, high: number): number;
function range(v: number): number[];
function times<T>(count: number, func: (index: number) => T): T[];
function remove<T>(array: T[], func: (v: T, index?: number) => any): T[];
function addWithCharCode(char: string, offset: number): string;
```

### Options

```javascript
// Write the game name to 'title'.
title = "CHARGE BEAM";

// 'description' is displayed on the title screen.
description = `
[Tap]     Shot
[Hold]    Charge
[Release] Fire
`;

// Define pixel arts of characters.
// Each letter represents a pixel color.
// (l: black, r: red, g: green, b: blue
//  y: yellow, p: purple, c: cyan
//  L: light_black, R: light_red, G: light_green, B: light_blue
//  Y: light_yellow, P: light_purple, C: light_cyan)
// Characters are assigned from 'a'.
// 'char("a", 0, 0);' draws the character
// defined by the first element of the array.
characters = [
  `
rllbb
lllccb
llyl b
`,
  `
  r rr
rrrrrr
  grr
  grr
rrrrrr
  r rr
`,
  `
 LLLL
LyyyyL
LyyyyL
LyyyyL
LyyyyL
 LLLL
`,
  `
   bbb
  bccb
bbllcb
bcllcb
  bccb
   bbb
`,
  `
l llll
l llll
`,
];

// Configure game options.
// options = {
//   viewSize?: { x: number; y: number }; // Set the screen size.
//   theme?: "simple" | "pixel" | "shape" | "shapeDark" | "crt" | "dark";
//    // Select the appearance theme.
//   isPlayingBgm?: boolean; // Play BGM.
//   isReplayEnabled?: boolean; // Enable replay.
//   seed?: number; // Set the random number seed used to generate sounds.
//
//   isCapturing?: boolean; // Capture a screen by pressing 'c' key.
//   isCapturingGameCanvasOnly?: boolean;
//    // Additional setting for isCapturing,
//    // will omit the margins on two sides when enabled.
//   isDrawingParticleFront?: boolean; // Draw particles in front of the screen.
//   isDrawingScoreFront?: boolean; // Draw the added score in front of the screen.
//   isShowingScore?: boolean; // Show a score and a hi-score.
//   isMinifying?: boolean; // Show a minified code to the console.
// };
options = {
  viewSize: { x: 200, y: 60 },
  theme: "pixel",
  isPlayingBgm: true,
  isReplayEnabled: true,
  seed: 1,
};
```

## Tips

- By drawing with `color("transparent")`, you can get the result of collision detection without drawing any shape on the screen.
- The collision detection is based on the drawing history of the shape. Therefore, even if a drawn shape is overwritten with a background-colored shape, the collision detection in that area will not disappear.
- The base value for the random seed for sound generation is generated from the `title` and `description` strings. If you want to use `seed` in `options` to adjust the generated sound, it is better to do so after the `title` and `description` are fixed.
- To improve the performance of the game, do the following (mainly for mobile devices):
  - Use `simple` or `dark` theme. Do not specify a theme that uses pixi.js (`pixel`, `shape`, `shapeDark`, `crt`) in options. WebGL post-effects may worsen performance.
  - Minimize drawing bars, lines, or arcs. They are drawn as a combination of many rectangles and highly detrimental to the collision detection process.
