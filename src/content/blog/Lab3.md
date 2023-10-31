---
title: 'HCI Lab 3'
description: 'Third lab in Human-Computer Interaction'
pubDate: 'Oct 09 2023'
heroImage: '/blog-placeholder-5.jpg'
---

Hello everyone !

Last week we took one step further the RollABall Game by converting it into an android version in order to play with it on our phones. You will find all the instructions on <a href="https://docs.unity3d.com/Manual/android-BuildProcess.html">this unity tutorial</a>.

Here are the steps to follow to do the exact same thing, you will see there is nothing difficult.


To begin, go in the Player Settings and the Build Settings,to configure your settings so that you game will have the runtime and properties you want.

Now you need to select your publishing format. First, select File then Build Settings. In the list of plateforms select Android.

Click Build. Select the destination for Unity to place the application. Click Save. This starts the build.

You will notice the game you have is not yet adapted for a smartphone. You have to do some modifications :

1) Change the camera view so you can see your game from the top.

2) If you want to use the accelerometer of your phone as an input you have to select you player, and in the inspector you create a new Player input (don't forget to suppress the previous one). Now your action should be a new one for example MobileInPut

3) Modify you PlayerController script as followed.
In the Start function add these lines :
```C#
    if (isMobileBuild)
    {
        InputSystem.EnableDevice(UnityEngine.InputSystem.Accelerometer.current);
    }
```
Change the FixedUpdate function to this :
````C#
Vector3 movement = Vector3.zero;
if (isMobileBuild)
{
    Vector3 a = UnityEngine. InputSystem. Accelerometer.current.acceleration.ReadValue();
    AccText.text = "Accelerometer" + a.ToString("F6");
    movement = new Vector3 (a.x, 0.0f, a.y);
}
else
{
    movement = new Vector3(movementX, 0.0f, movementY);
}

rb.AddForce (movement * speed);
````


##### You should now be able to play your game on your phone !

