# tf2-turnstacking-script
TF2 Script that allows you to use +left and +right during charging 

## Why use this one over the 100 others? 
Every single other turnbind script has the same issue which is made clear in [this video](https://youtu.be/nFLDW96VliU).
Essentialy the problem is that you need to repress A or D during and after your charge to start turning and/or strafing after.
My version fixes this by having the script detect when you are holding down a key instead of just when you press and release. This allows it to always either turn or strafe depending on whether you're charging or not without having to let go and repress the key.



## How to use 
When in-game, press your charge toggle key (default bound to B) and you should hear demoman say either Yes or no. This is how you know if the script is currently running.
When charging, you need to hold down your charge button ( whether this is right click or your jump charge bind ) and a and d will now be rebound to +left and +right
This is an improvement from previous turnbind scripts as you no longer need to release and repress a or d to start turning and when you finish the charge you dont need to repress to start air strafing.


## How to install 
1. Put the turnbindv2 script into "YOURSTEAMDIR\steamapps\common\Team Fortress 2\tf\cfg" and rename it to exactly "turnbindv2.cfg".
2. Open up demoman.cfg inside of the cfg folder, if demoman.cfg does not exist, create it by making a plain text file and renaming it to demoman.cfg. 
	 If you are using a custom hud or are using mastercomfig, create a folder called "overrides" and put demoman.cfg in there 
	 If you do not have an anti-ghosting script put antighosting.cfg into your cfg folder 
3. Inside of demoman.cfg, type "exec turnbindv2"
4. When you pick the demoman in-game you should now see a message saying the turnbind script has ran in the console 

## How to customize 

You can change your charge toggle key and jumpcharge key at the top of the script. 
If you normally have your jumpcharge button bound to something else, you can rebind it next to disableJumpCharge 
I have m_filter to be enabled and disabled when charge is held down, if you do not want this find the +charge alias and remove m_filter from the end of it
