# Unity Maze Game
A 3D maze game built in Unity where the player tilts the maze to roll a ball to the end goal. Built as part of Assignment 2.

 How to Play
Use the on-screen arrow buttons (bottom-left and bottom-right) to tilt the maze left and right
Roll the ball through the maze without falling off
Reach the ball at the end to trigger the "You Win" sound!


How It Was Built
Maze Structure
Built using scaled cubes (15X, 1Y, 1Z) to create long rectangle walls
Key objects: Ground, Head, Right Wall, Left Wall
A custom material called "border" was created to colour the maze walls
Additional inner walls were added at varying sizes and heights to increase difficulty
Some rectangles were tilted for an extra challenge (attempted challenge)

Physics & Controls
A Plane object with a custom glass material acts as a transparent barrier, keeping the ball inside
UI Buttons (arrows styled as =>) are placed bottom-left and bottom-right using Rect Transform settings:

Pos X: 60, Pos Y: 60, Pos Z: 0
Width: 100, Height: 100, Pivot: (0.5, 0.5)


Each button applies a constant force to move the maze left or right (opposite directions)
A Parent object groups all maze elements so the whole maze moves as one
A Superparent was added to apply additional constant force when more objects were added

Freeze Settings

Position and rotation are frozen on the parent to prevent unintended movement


Assets Used
All assets used are free:
AssetSourceLow poly sky backgroundFarland Skies – Low Poly by Borodar (Unity Asset Store)Nintendo-style arrow iconsUX Flat Icons by Heathen Engineering (Unity Asset Store)Background music"Getting Ready" by Ahjay Stelino (Mixkit)Win sound effect"Game Level Music" (Mixkit)
Audio Setup

Background music is attached to the Main Camera so it plays immediately on start
Win sound is attached to the Player (ball) and only triggers when the ball is clicked at the end


 Built With

Unity
C# scripting
Unity Asset Store (free assets)
Mixkit for audio
