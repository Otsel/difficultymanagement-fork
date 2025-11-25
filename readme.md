# DifficultyManagement Fork

This repository is a fork of Difficulty Management by Author: [zmolahah](https://www.spigotmc.org/resources/authors/zmolahah.17091/)

I am merely updating this script to work with modern versions of Minecraft and Skript.

**Current Version Supported: 1.21.10**

 [Skript](https://github.com/SkriptLang/Skript) server plugin is required.

Readme by zmolahah:

> **Description:**   Simply put this allows you to change the difficulty per-player without effecting PVP. For example someone on easy difficulty would not have an advantage over a player on hard mode since it only effects mob damage.     
> 
> **Features:**  
> 
> -   permission support
> -   configuration
> -   allows player's to have a unique difficulty
> -   supports peaceful, easy, normal, hard and hardcore
> -   easy players will not have an advantage over hard players
> 
> **Installation:**  
> 
> 1.  Download [Skript](http://dev.bukkit.org/bukkit-plugins/skript/). This works with
> [2.2](http://dev.bukkit.org/bukkit-plugins/skript/forum/misc/72732-skript-2-2/#posts)
> 2.  Run your server to generate the Skript folder, go into the Skript scripts folder and add difficultyManagement.sk
> 3.  Use /sk reload difficultyManagement.sk
> 
> When you have successfully installed the script it will set your
> server difficulty to hard. The server will not act like hard to people
> not in hard mode but the server actually has to be in hard mode in
> order for this script to work     
> **Peaceful:**   Players in peaceful will not lose hunger. Hostile mobs will not attack the player.     
> **Easy:**   Players in easy can not starve below 5 hearts, hostile mobs will deal half damage     
> **Normal:**   Players in normal can not starve below half a heart, hostile mobs will deal 25% reduced damage     
> **Hard:**   Players in hard will starve to death, hostile mobs will deal full damage     
> **Hardcore:**   Players in hardcore will starve to death, hostile mobs will deal full damage. If the player dies they will be banned from the
> server     
> **Configuration:**  
> 
> -   [default:normal] Default Difficulty - (peaceful, easy, normal, hard, hardcore) This is what new players difficulty will be set to
> -   [default:false] Zombies Break Doors - (true or false) if enabled zombies will be able to break doors just like in hard mode
> -   [default:false] Use Permissions - (true or false) if enabled players will require a permission node to set their difficulty. See
> permissions
> -   [default:false] Require OP - (true or false) if enabled only people with OP can set their own difficulty
> -   Permission Message - type your own permission message for if the person is not OP or does not have permission. Requires Require OP or
> Use Permissions to take effect
> -   Hardcore Ban Message - type your own message to display to players who get banned when they die in hardcore mode
> -   [default:false] Disable PVP in Peaceful - if enabled you will not be able to attack or be attacked by players while in peaceful
> 
> To reload configuration at any time just use /sk reload
> difficultymanagement     
> **Permissions:**  
> 
> -   difficultymanagement.peaceful - allows players to use /dm peaceful
> -   difficultymanagement.easy - allows players to use /dm easy
> -   difficultymanagement.normal - allows players to use /dm normal
> -   difficultymanagement.hard - allows players to use /dm hard
> -   difficultymanagement.hardcore - allows players to use /dm hardcore
> 
> **Commands:**  
> 
> -   /difficultymanagement (or /dm) - shows your current difficulty
> -   /difficultymanagement (or /dm) <peaceful/easy/normal/hard/hardcore> - change your difficulty

