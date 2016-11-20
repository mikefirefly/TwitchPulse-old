# TwitchPulse

TwitchPulse v1.0
PCGambler 2016, FREEWARE

INTRO
-----
A simple desktop application that notifies the user when a specific channel goes live. Created as I couldn't find a Twitch notifier tailored to my requirements, ie. one that:
- is simple (no chat etc.)
- is light on system resources (takes less than 20MB of RAM while eg. Chatty will happily eat up 300MB+)
- is not limited to followed channels (not tied with a twitch user account)
- most importantly, uses configurable sound notifications - specifically, is able to emit a specific sound once a specific caster goes live

USAGE
-----
Monitored channels are defined via CASTERS.txt file. Each entry (line) defines a stream watchdog. Entries starting with semicolon (;) are ignored (useful for comments).
	
When a channel goes online or when a live channel's game/title changes, the application:
* shows a notification window with caster(s) name(s) and game(s)
and/or
* plays a sound which is configured in CASTERS.txt file. An example CASTERS.txt file is distributed with the application and contains examples.

The general entry format is:

- MyFavouriteCaster^mfc.wav^My Favourite Caster!  - when "MyFavouriteCaster" goes live, display a notification with "My Favourite Caster!" text and play mfc.wav file from the "Sound" folder (if the file exists)
- SecondCaster									                  - when "SecondCaster" goes live, display a notification with "SecondCaster" text and say "SecondCaster" phrase
- ThirdCaster^-^Just another caster								- when "ThirdCaster" goes live, display a notification with "SecondCaster" text and do not notify via sound
- Example^Example is live!^FriendlyName			      - when "Example" goes live, display a notification with "FriendlyName" text and play say "Example is live!" phrase

ADDITIONAL INFORMATION:
-----------------------
*Right clicking the channel list allows to configure the program (colors, fonts etc.)
*Channel status is checked every 60 seconds, this interval is not configurable
*When a live channel goes offline, it's not announced in any way
*Double clicking on the list item opens the caster channel in default browser or using external player (if configured in Preferences)
*Clicking on a notification makes it disappear
* Taskbar icon:
	* turns red if there are new live channels since last update
	* turns gray if there are no live channels
	* shows live channel count (+ when more than 9)
	* shows X when there is a network problem


FINAL WORDS - PLEASE READ
-------------------------
Even though I did my best to fix potential problems and squash all bugs, I cannot be sure that the application works flawlessly. Therefore I can't be deemed responsible when something goes wrong.
However, feel free to send feedback, questions, feature requests to pcgambler@o2.pl

Finally - if for some reason you would like to tip me, the proper PayPal address to do so is pcgambler@protonmail.com Thanks!
