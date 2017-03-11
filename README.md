# MouseTrap
#YouTube Link:
https://www.youtube.com/watch?v=vnOmjXZNpLE

Inspired by Tom and Jerry I tried to build a Mouse Trap that works with simple tasks that are linked together to produce a domino effect in which activating one device triggers the next device in the sequence. I am using not only physics but also animations for some assets. First problem that I faced was friction between two objects. In unreal engine it take and average value between touching materials. In order to make and object move smother on a surface and not to stop in the middle I created a custom physical material which can be used and added to any material that already exists. Physical material allowed me to change the friction value and make object slide.
![Friction](https://github.com/Leylamammadova/MouseTrap/blob/master/screenshots/friction0.gif)

This allowed me to finish the first sequence of events. Mouse(in our case its a ball) steps on a platform with cheese, platform gets activated and by force applied on a plank a huge tube kicks the box that slides down on another plank untill the staircase is reached.
Next event: dominoes that fall on the stairs that hit a sphere.
Next event: sphere colides with a ball that swings on a rope. In order to connect spheres on a rope I used constraints. Physical constraints actors are connected by the centers of spheres. To make is look like a rope I used cable actor, again connected in centers.
![Constraints](https://github.com/Leylamammadova/MouseTrap/blob/master/screenshots/B1ajZI.gif)

When sphere collides with golden cube(button) it has button pressed effect and triggers an animation of oppening box full of zombie ragdolls. There are physical assests of sceletal mesh. I got it from MIXAMO. 
![Zombie](https://github.com/Leylamammadova/MouseTrap/blob/master/screenshots/blKQPn.gif)

Their bodies fell on a balance scale (just two plane cubes connected together) which activates animation of balance scale which also triggers the hammer to smash our mouse(ball). For hammer I also used animation. 





