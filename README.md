# Galaxy Invaders

> **Overview**
>
> This is a Arcade Game Engine rewritten entirely in Javascript. You can play
> the sample game on [http://patnaikshekhar.github.io/GalaxyInvaders](http://patnaikshekhar.github.io/GalaxyInvaders)
>
> The engine is written in vanilla javascript and only uses require js as an
> external library.
>
> The main file is called by require JS which in turn references the game engine. The engine consists of a main game object which can be initialized as
>
```js
new Game('game', Constants.WINDOW_WIDTH,
      Constants.WINDOW_HEIGHT, Constants.FPS, Constants.SPEED_UP);
```
>
> Each game consists of scenes which must inherit from scene.js in the engine
> A scene can be started by running
```js
game.startScene('menu');
```
>
> Each scene consists of Scene Objects. These are the actual objects in the game such as Ships/Enemies/Bullets etc
> The scene objects must have 3 methods - draw, update, keyPress. The draw method is called to draw on the buffered canvas. The update is used to update the game state and the key press method is used to handle input.
