# ai-3d-maze

Basic game for walking through generated mazes (developed in Chat GPT-5).


## Overview

This game generates a maze, and the player can navigate through the maze from start to finish. This isn't intended as a full fledged game - players can navigate through the maze, but there are no timers, no obstacles, no enemies. The intent is for this to be a base version of a game, and to derive full games from this.


## Directions

There are two windows to look at on the screen. On the left-side is a 3D view of the maze, seen from the perspective of the player. On the right-side is a 2D view, looking top-down on the maze. In the 2D view, the map gets automatically updated based on what you see in the 3D view. Both windows represent the same maze, from a different point of view.

The controls for the game are the arrow keys. Left and right arrow turn 90 degrees in the matching direction. The up arrow steps one square forward. You cannot walk through walls, and there are no ways to get through a wall.

Looking at the 2D map, the player will always start in the upper-left corner of the map. The goal is to get to the lower-right corner of the map. The exit stands out - it is green.

In the upper-right corner above the game, there is a button to change the size of the map. Changing the selection automatically restarts the game at that new size.

In the lower-right corner under the game, there is a Reset Maze button. When the player has made it to the exit (in the lower-right corner), clicking the Reset Maze button starts a new game. A new maze is generated, and the player moves back to the top-left corner.


## Details

Truly, this is intended as a basis for "true" games being implemented. The alternates will use this the initial version. Each alternate will be modified for what's needed.

This application uses Depth-First Search as the algorithm to generate the map. Each map will utilizes all the available squares. Also, there are never any loops. This is fine: a good starting point that might change in an alternate game.


## From Release #1 (Build 14 on 2/2/26)

* Game generates maps where each map is rendered with a 2D and 3D view.

* The walls are red, with the exception of the exit, which is green.

* The particular shade of colors of the walls darken based on distance.

* Provide a modal that allows the map size to change.

