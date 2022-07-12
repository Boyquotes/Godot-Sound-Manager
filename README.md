# Godot Sound Manager
An easy and optimized way to manage your sound effects in the Godot Game Engine! Just extract **GodotSoundManager.zip** and place inside the **addons** folder of your Godot project!

Download the demo to see the most basic functions in action!

# Variables

**MASTER -** The master audio bus

**DEFAULT -** The default audio group

**muted_groups -** Keys are all sound groups, values are whether or not the group is muted (booleans)

# Functions
**request(stream, group=DEFAULT, bus=MASTER, pitch=1, position=0) -> AudioStreamPlayer:**

Plays an AudioStreamPlayer with variables corresponding to function values if the group is not muted

**set_mute(value, group=DEFAULT) -> void:**

Changes whether or not the group it muted to value

**get_mute(group=DEFAULT) -> bool:**

Returns muted value of group if group is in **muted_groups** dictionary, otherwise returns null

**stop(group=DEFAULT) -> AudioStreamPlayer:**

Stops all AudioStreamPlayers in group

**get_player_volume(player) -> float:**

Returns the bus volume of the player

**set_player_volume(player, value) -> void:**

Sets the bus volume of the player to value

**get_bus_volume(index) -> float:**

Returns the volume of the bus at index

**set_bus_volume(index, value) -> void:**

Sets the bus at index's volume to value

**play(player, stream, bus=MASTER, pitch=1.0, position=1.0) -> void:**

Forces player to play with variables corresponding to function values *NOTE: IGNORES MUTING*

**delete_invalid() -> void:**

Deletes items in **players** array that are not of type AudioStreamPlayer

**update(new_count) -> void:**

Changes the length of **players** array to new_count

**free_in_queue(interrupt=true) -> void:**

Deletes players in **free_queue**
