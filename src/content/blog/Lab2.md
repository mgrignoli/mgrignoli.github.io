---
title: 'HCI Lab 2'
description: 'Second lab in Human-Computer Interaction'
pubDate: 'Oct 03 2023'
heroImage: '/ennemy.png'
---


Hello everyone !

Today I completed a Unity tutorial to create my first 3D game. You can also do it ! As a beginer myself, I found it very comprehensible and easy to complete. Follow <a href="https://learn.unity.com/project/roll-a-ball?uv=2022.3">this link</a> !


#### First of all, I invite you all to create the environnement of the game :

1) Create the ground with a 3D object Plane. Set its scale to X=2 Y=2 Z=2. Then in the assets, create a folder Materials where you add the first Material named ground. You can choose the color you want in the inspector and the you drag the material onto the ground in the scene.

![blog placeholder](/ground.jpg)

2) Now create in the hierarchy an empty object named Walls. Inside it you will put the four walls of the game. To create a wall, add a 3D object Cube and rescale it : X=0.5 Y=2 Z=20.5. Then you just have to duplicate this wall 3 times and place them following these different positions : 

X=-10 Y=0 Z=0
X=0 Y=0 Z=10
X=10 Y=0 Z=0
X=0 Y=0 Z=-10

You can also create a nex material with a differnt color in the forlder Materials and dra it onto the walls in the scene or in the hierarchy.

![blog placeholder](/walls.jpg)

3) Then for your player, create a 3D object Sphere and color it the way you want using the same method as before.

![blog placeholder](/player.jpg)

4) Finally, you have to create the PickUp objects. For that create an empty object in the hierarchy naled PickUp Parent. Then add a Cube to the scene and rename it PickUp, scale it to X=0.5 Y=0.5 Z=0.5, and color it the way you want with the materials folder. In the assets create a new forlder named Prefabs. You can now drag your PickUp object inside it. Thank to this prefab you can now duplicate the collectibles as many time as you want by dragging it in the scene. Staying on you prefab PickUp, in the inspactor, you have to add a Tag named PickUp and the select it.

![blog placeholder](/Tag.png)

![blog placeholder](/game.jpg) ![blog placeholder](/ennemy.png)





####