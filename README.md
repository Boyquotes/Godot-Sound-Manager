# Godot Sound Manager
An easy and optimized way to manage your sound effects in the Godot Game Engine!
Download the demo to see the most basic functions in action!

# Variables

||MASTER|| - The master audio bus

DEFAULT - The default audio group

muted_groups - Keys are all sound groups, values are whether or not the group is muted (booleans)

# Functions
request(stream, group=DEFAULT, bus=MASTER, pitch=1, position=0) -> AudioStreamPlayer:

Plays an AudioStreamPlayer with variables corresponding to function values if the group is not muted


