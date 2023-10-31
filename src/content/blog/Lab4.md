---
title: 'HCI Lab 4'
description: 'Foirth lab in Human-Computer Interaction'
pubDate: 'Oct 27 2023'
heroImage: '/blog-placeholder-2.jpg'
---

Welcome back!

In this post, I'm excited to guide you through the process of adapting your Rollaball application for virtual reality (VR) gameplay. In our last lab of HCI, we had a hands-on experience using Oculus VR headsets, which offer an immersive experience, elevating gaming to a whole new level.
I've outlined the steps to get you started. You can also use <a href="https://developer.oculus.com/documentation/unity/unity-tutorial-hello-vr/">this website</a> to help you with the setting up.


Making the Rollaball game work in virtual reality started with getting the game size just right for VR play. We wanted players to grab and interact with the game board, so adjusting its size was crucial. Once that was sorted, I found a room setup in the Unity Asset Store—a cozy room with a bed. I placed the Rollaball game board on the bed within this virtual space. While I went with this ready-made setup, you can get creative and design your own environment using Unity's tools. The main aim is to create an awesome space where players can dive into the Rollaball game in VR.

Here is a picture of my room :


Once that was done we delve into the technical aspect to make the game playable in virtual reality.


- In the package manager, install OpenXR Plugin an XR Interaction ;
- In Edit go to Project settings select XR Plug-in Management,and tick OpenXR ;
- In the project windox, follow the path Assets > Samples > XR Interaction toolkit > 2.2.0 > Starter Assets and for each asset, in the inspector, select the button Add to ActionBasedContinousMoveProvider default ;
- In the Hierarchy, create an XR Origin, by right clicking XR> XR Origin VR and in the inspector, add Character Controller and Character Controller Driver to the XR Origin ;
- Right click in the Hierarchy, go to,XR > Locomotion System (Action based) and drag and drop it in the Charactor controller driver in the inspector for the XR Origin ;

Your inspector for XR Orignin should be the same as this one : 


- Now you have to set you Right and left HandController as follow : 


- Create an empty Prefabs (HandContoller) in the Prefabs folder, add a cube and a cylinder as below ;


- For left and right handController, in the Inspector remove XR Interactor, Line Rendere and XR Interactor Line Visual. Create an empty GameObject called ModelParent under the HandController, add the created Prefabs and ModelParent, add a sphere Controller to your handControllers ;

- 








