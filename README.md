# Unity-Pathways

This repository includes playable builds for my implementation of Prototypes and Challenges 1-5 of the Unity Pathway Junior Programmer.

To run:

Download a .zip file and extract the contents. Open the `Build` folder and open the respective Unity Application file.

### Prototypes

Prototypes are the main projects that taught how to develop certain aspects of games. My implementation also includes the Bonus Features provided by the Pathway program.

* **Driving Simulator** - Local multiplayer driving simulation where you can control two tanks and drive down a road with obstacles

* **Food Stampede** - Shoot food at an oncoming stampede of animals

* **Parkour** - An infinite run and jump game
  * Press `Space` to jump, double tap to Double Jump
  * Hold `LeftShift` to run faster
  

* **Sumo Battle** - Knock off enemy waves from the battle ring using brute force and power-ups
  * Power-ups will periodically spawn on the arena. There are three different power-ups:
    * Rockets - Green Diamond
      * Press `F` to shoot rockets at enemies
    * Pushback - Yellow Diamond
      * Increases force you hit enemies with
    * Smash - Brown Diamond
      * Press `Space` to rise and smash the ground, knocking back enemies in the area
  * Every 2 rounds, a boss will spawn that repeatedly spawns enemies until it is taken out

* **Fruit Ninja** - Slice the fruit, avoid the bombs

### Challenges

Challenges are meant to practice the skills learned from their respective Prototypes in a brand new scene. You are required to fix the bugs within the game
using your knowledge of C# scripting and Unity.

* **Plane Simulator** - Fly a plane through some obstacles

* **Fetch** - Send out your dog to catch the balls dropping from the sky

* **Balloon Bomb** - As a balloon, avoid the bombs and collect money

* **Soccer** - Knock the oncoming soccer balls into the other goal while defending your own goal

* **Whack-a-Food** - Click the food and avoid the skulls to earn points

### Pathways Part 2

This section is the second half of the Junior Programmer Pathway that focused on more complex topics and tools rather than true game development. This section included source control setup in Unity, managing flow and data between scenes and sessions, object-oriented principles, and optimizations tools.

* **Resource Management Simulator** - Produce resources and ship them out.
  * In the menu screen, you can select a color of the forklifts in the game scene.
    * You can save this color by pressing the Save button, which will save this color for future sessions.
    * You can load the last saved color from a previous session by pressing the Load button.
  * In the game scene, you can select different units to see their information.
    * You can left-click a forklift and right-click on a resource to make the forklift collect and drop off the resource at the shipping area.
    * You can left-click the person and right-click on a resource to make the person move to the resource and increase its production rate.
  * You can go back to the menu and change, save, or load colors at any time.

* **Optimization** - 2000 forklifts rotate and move around the scene.
  * This project had me use Unity's Profiler tool to track down the cause of the tanked performance. Eventually, I tracked down the cause to be the Move() method, which took approximately 90ms to complete every frame, which heavily dropped performance. Once it was fixed, performance was significantly improved (about 70 FPS difference).
