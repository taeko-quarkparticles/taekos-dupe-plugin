# Taeko's Dupe Plugin
a fairly simple dupe checker.
/dupe - view list of locations containing chests with deemed valuables.
/dupe clear <number/found> - clear the list. if you enter a number after "clear", it will clear just that number item from the list, and add it to a list of locations that should be ignored. to clear the list of found locations that should be ignored, use "/dupe clear found".

Example:

Player Command: /dupe

-----[Skysucht - Dupe]-----
==== X: 0 Y: 64 Z: 134 ==== 0
==== X: 75 Y: 64 Z: 543 ==== 1
==== X: 85 Y: 64 Z: 14 ==== 2
-----[Skysucht - Dupe]-----

Player Command: /dupe clear 1
-----[Skysucht - Dupe]-----
==== X: 0 Y: 64 Z: 134 ==== 0
==== X: 85 Y: 64 Z: 14 ==== 1
-----[Skysucht - Dupe]-----
Player Command: /dupe clear
-----[Skysucht - Dupe]-----
-----[Skysucht - Dupe]-----
Chunks are searched as generated by the player. If a chest has items put in it, they will only register once that chunks has been fully unloaded and reloaded, in other words, when the player leaves and comes back.
