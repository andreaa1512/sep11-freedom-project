# Entry 5
##### 05/06/24

So far I have the basics. The basics being the floor, the sprites and basic commands. To really finish my MVP I need to give the sprite more complicated commands. The duck and hw sprites have a different “job”. The duck has to make the collector gain a point when they touch a duck. When the collector touches a hw sprite then the game lost scene shows up. The duck and hw sprite have to also spawn at a random point of the screen. Using `Math.random()` along with more code will randomly select between the duck and hw sprite. Then for them to have a different “job” this bunch of code would do the trick


``` Javascript
if (obj.isColliding(collector)) {
       if (obj.sprite === "duck") {
         score += 1;
         destroy(obj);
         scoreText.text = `Score: ${score}`;
       } else if (obj.sprite === "hw") {
         go("gameOver"); // transition to the game over scene
       }
     }
```
 With that code it will detect whether it is a duck or a hw and then do the action needed.



[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)