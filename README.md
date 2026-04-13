# Sky-Orb-Collector_Gnana

**I used AI as a development assistant, but the game design, structure, and requirements were defined by me.**

**To run the GAME downlaod the following files:
SkyOrbCollector_Game.html
SkyOrbCollector_Manual.html**


For more details please refer to the SkyOrbCollector_Manual.html


**This is the prompt I gave an AI engine as per the assignment requirements:**

I need you to build a complete, clean, and fully functional mobile VR game using A-Frame that works on desktop, mobile phones, and Google Cardboard-style VR.

Game Title: Sky Orb Collector
Game Concept:
The player is placed in the center of a 3D sky environment. Floating orbs appear around the player. The player collects orbs by gazing at them (no hand controls). When the player looks at an orb for a short duration, the orb disappears and the score increases.

Core Requirements (MUST IMPLEMENT ALL):
1. Flash Screen (Start Screen)
* Display game title: "Sky Orb Collector"
* Display author name: "Gnana Deepika"
* Include a "Start Game" button
* Simple clean UI in A-Frame
  
2. Setup Menu
* Toggle for background music (ON/OFF)
* Option to select Level 1 or Level 2
* Start button after selection
  
3. Gaze-Based Controls
* Use A-Frame cursor with fuse:
   * fuse: true
   * fuse-timeout: ~1500ms
* Player interacts ONLY by looking at objects
  
4. Scoreboard (Always Visible)
* Show:
   * Score
   * Timer (countdown)
* Fixed position in front of camera
  
5. Two Levels
Level 1 (Easy Mode):
* Light sky background (blue)
* Slow-moving orbs
* Only collectible orbs (no penalties)
Level 2 (Hard Mode):
* Dark/stormy sky
* Faster orbs
* Include "bad orbs":
   * Reduce score when collected
   * Different color (e.g., red)
     
6. Game Mechanics
* Orbs spawn randomly around the player
* When gazed at:
   * Orb disappears
   * Score updates
   * Sound effect plays
* Timer countdown (e.g., 60 seconds per level)
* End screen when time finishes:
   * Show final score
   * Option to restart or go to next level
     
7. Sound Effects
* Background music loop (toggleable)
* Collect sound (pleasant "ding")
* Wrong orb sound (error/buzz)
  
8. Objects with Textures (IMPORTANT)
* DO NOT use plain colors only
* Use textured materials (e.g., glow, gradients, galaxy textures)
* Use with texture maps
  
9. Collision / Interaction
* Use raycaster + cursor for gaze detection
* No keyboard or mouse clicking required
  
10. VR Compatibility
* Must support:
   * Desktop (mouse look)
   * Mobile (gyro movement)
   * VR split-screen (stereoscopic view)
     
Technical Requirements:
* Use pure HTML + JavaScript + A-Frame
* Keep everything in one HTML file if possible
* Write clean, commented code
* Use reusable components for:
   * Orb spawning
   * Score tracking
   * Timer
     
Additional Features (if possible):
* Slight animation (floating orbs)
* Smooth transitions between levels
* Simple UI panels using A-Frame planes
* Random spawn positions within a radius

Constraints:
* No violence or blood
* Keep gameplay simple and achievable
* Do not use external frameworks other than A-Frame
* Avoid overly complex physics
