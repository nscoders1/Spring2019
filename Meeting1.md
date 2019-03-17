
# Introduction & Plans -- Dave M.C.'s 

# Examples of our Destination
1. [Space Invaders](http://annotated-code.maryrosecook.com/space-invaders/index.html) by Mary Rose Cook
2. [Pong](https://nscoders1.github.io/pong/game.html) by Marc-André Cournoyer
3. [Breakout](https://end3r.github.io/Gamedev-Canvas-Content-Kit/demos/lesson10.html) by Andrzej Mazur


# Lessons

1. Login to github and clone https://github.com/nscoders1/Spring2019
   1. We'll be doing a lot of work in the web browser
1. We want students to understand https://nscoders1.github.io/Spring2019/1.html 
   1. Source at https://github.com/nscoders1/Spring2019/blob/master/1.html
2. Let's create a function for drawing the rectangle: 
```
  function drawRect() {
    ctx.beginPath();
    ctx.rect(20, 40, 50, 50);
    ctx.fillStyle = "red";
    ctx.fill();
    ctx.closePath();
  }
  ```

After the `canvas.getContext("2d");` line add a call to your new function.  It should look like this:
  ```
    var ctx = canvas.getContext("2d");
    drawRect(20, 30);
  ```

4. But it always puts the rectangle in the same place, so let's add variables:
```
  function drawRect(x,y) {
    ctx.beginPath();
    ctx.rect(x, y, 50, 50);
    ctx.fillStyle = "red";
    ctx.fill();
    ctx.closePath();
  }
  ```
After the `drawRect(20, 30);` line add a call to your new function a second time with different parameters.  
It should look like this:
  ```
    var ctx = canvas.getContext("2d");
    drawRect(20, 30);
    drawRect(120, 130);
  ```


