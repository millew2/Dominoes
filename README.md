Domsim
======

A Dominoes Simulator

User Guide
----------

The two topmost buttons in the menu will bring you to Draw Mode and Run Mode, respectively.

In Draw Mode, you can draw a line on the canvas which will segment into distinct dominoes upon releasing the mouse button.

In Run Mode, you will see the currently loaded line of dominoes in 3D with red wireframe dominoes on a blue floor.

In either mode, you can click the "Load Setup" and "Save Setup" buttons to load the most recently saved domino setup and save a new one, respectively.

In Run Mode, you can click "Play Sequence" to begin tilting the first domino and start the sequence of toppling. You can also click "Reset Dominoes" to reset all dominoes to a standing position. Finally, you can click "Freeze" at any time during the falling of dominoes to freeze or un-freeze their motion.


Implementation Manual
---------------------

We chose to use a single strip of dominoes to simplify physics simulation and camera control. With one line of dominoes, we can allow the camera to follow the one lead domino at any given moment, and we can concern ourselves only with collision detection between adjacent dominoes. We hope to change this in the future and allow for branching paths and even completely separate strips of dominoes. We chose wireframe dominoes because there was an issue with lighting where dominoes were all lit as if they were standing in the standard position, facing the positive x axis at the origin. We hope to improve the lighting in the future to remedy this and create a better overall 3D visual experience. We chose to use an older version of OpenGL because it is what we used in class and were familiar with; however, we hope to port it to the newest version to keep up with standards.
