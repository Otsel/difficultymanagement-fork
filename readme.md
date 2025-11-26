# Per-Player Difficulty Management

This repository is a fork of [Difficulty Management](https://www.spigotmc.org/resources/difficulty-management.12131/) by [zmolahah](https://www.spigotmc.org/resources/authors/zmolahah.17091/). 
I am merely updating this script to work with modern versions of Minecraft and Skript.

**Current Version Supported: 1.21.10**

**Dependencies:**
 [Skript](https://github.com/SkriptLang/Skript) server plugin is required. Runs on Paper or Purpur.



**Description:**   This server-side plugin allows players to choose their own difficulty on a per-user basis. These settings do not conflict, and allow each user to play how they want to play!

**Features:**  

-   Allows each player to set their *own* difficulty, and each can be set differently at the same time.
-   Compatible with your favorite permissions plugin.
-   Highly configurable, tailor your own experience.
-   Supports not just Easy, Normal and Hard, but also Peaceful and Hardcore (for the insane).
-   PvE only! Does not impact PvP damage, nor will it conflict with PvP plugins.

**Installation:**  

1.  Download [Skript](https://github.com/SkriptLang/Skript) and drop the .jar file in your server's plugins folder.
2.  Run your server to create the Skript folder, move `difficultyManagement.sk` into `\plugins\Skript\scripts` directory
3. Stop the server
4. Edit `server-properties` so that `difficulty=hard`
5. Restart the server

**Note:** This plugin **requires** that your server difficulty be set to hard, as it works by utilizing hard difficulity stats and scaling *down* mob damage and hunger if otherwise set to lower difficulty.



|  Difficulty|Mob Damage  | Hunger |Perma Death| 
|--|--|--|--|
| Peaceful |  Mobs ignore player| Player will not lose hunger |❌
| Easy | 50% |Player cannot starve below 5 hearts  |❌
| Normal | 75% | Player cannot starve below ½ heart |❌
| Hard | 100% |  Player can starve|❌
| Hardcore | 100% | Player can starve|✅*

**Player is server banned upon death.*

**Configuration:**  
-   [default:normal] Default Difficulty - (peaceful, easy, normal, hard, hardcore) This is what new players difficulty will be set to
-   [default:false] Zombies Break Doors - (true or false) if enabled zombies will be able to break doors
-   [default:false] Use Permissions - (true or false) if enabled players will require a permission node to set their difficulty. See permissions
-   [default:false] Require OP - (true or false) if enabled only people with OP can set their own difficulty
-   Permission Message - type your own permission message for if the person is not OP or does not have permission. Requires Require OP or Use Permissions to take effect
-   Hardcore Ban Message - type your own message to display to players who get banned when they die in hardcore mode
-   [default:false] Disable PVP in Peaceful - if enabled you will not be able to attack or be attacked by players while in peaceful

To reload configuration at any time just use `/sk reload difficultymanagement`     

**Permissions:**  

-   `difficultymanagement.peaceful` - allows players to use /dm peaceful
-   `difficultymanagement.easy` - allows players to use /dm easy
-   `difficultymanagement.normal` - allows players to use /dm normal
-   `difficultymanagement.hard` - allows players to use /dm hard
-   `difficultymanagement.hardcore` - allows players to use /dm hardcore

**Commands:**  

-   `/difficultymanagement` (or `/dm`) - shows your current difficulty
-  `/difficultymanagement` (or `/dm`) `peaceful/easy/normal/hard/hardcore` - change your difficulty
