## Devtober Game Jam Post-Mortem
### Developer: John Cotton
### Game: Candlestick Jump
---
Goal: To create a 2d platformer where you try not to burn your butt while jumping over candlesticks.

#### About the tech stack
I just recently discovered GB Studio as an option for building games. While I have considered it for a top down RPG style game, the platformer style option added in Beta 2 proved to be the right choice for this concept. In retrospect, this engine is an excellent tool to build many different types of games.

#### Graphic Design: 
Most of the assets in this game are stock assets borrowed from the GB Studio Boiler Project. However, there was a bit of background editing involved. I tried many programs to develop a good clean workflow. Aesprite stood out as the most intuitive of the tools for editing the png backgrounds, and for creating the player sprites.

#### Music and SFX:
The biggest struggle in this process for me was making the music. I tried for several days to avoid penciling in every note in MilkyTracker (I'm on a mac). I tried using Midi, I tried syncing my external midi devices, and I tried many other apps in the process. The workflow I locked in on in the end was to use Milky Tracker as designed with the sounds provided in the template.mod file, but using an external midi keyboard to add the notes to each channel. The preview in GB studio is a really nice feature as the sounds are not 100% accurate between MilkyTracker and GBStudio.

#### Key Takeaways:
##### 1. Aesthetic is everything
Creating an awesome aesthetic is likely the most challenging part of creating a game in GB Studio. We did not achieve anything unique, but the next attempt will have a heavy focus on aesthetic.

##### 2. D.R.Y. (Don't repeat yourself)
A foundational principal of Software Design is to avoid duplicating logic. Custom Events are an amazing way to avoid repeating logic throughout levels. Finding yourself using the same logic multiple times? Consider using a Custom Event to handle this logic. Then you can update in one place, and it will automatically update everywhere.
I started off with a ton of duplication, and my last refactor had me removing about 80% of my scripts because I could accomplish the same thing inside a custom event, as well as using collision groups.

##### 3.  Version Control (Never lose a line of code)
I checked this project into a git repository at the beginning. This allowed me to make many changes over time, and periodically backup my project. This not only allows me to backup my code on github, but I can now time travel through my changes over time and see any state that I checked into a commit.

##### 4. The actual hardest part
The hardest part of this project was sitting down and putting in the work to make it happen. After getting a good build going itch.io makes it easy to distribute the game to friends and family to get some good test cycles.
