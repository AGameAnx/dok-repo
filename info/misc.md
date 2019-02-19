# Miscellaneous Information

## Replays
To share replays, share the `.dokreplay` and the `.dokreplayx` file with the same name.
The `.dokreplayx` file contains the layout and patch used on the map so that replays have the required information to work.

## Map Names
Map names now have the format of `<map name> [<min players>,<max players>]`.
For example, `Kalash Site [2,6]` means that the map can be played with any number between 2 and 6 players.
The map will change depending in the number of players so that you may play a 1v1, 2v2 or 3v3 without having extra resource patches (unless there are uneven teams).
Team mode maps may only know if a 1v1, 2v2 or 3v3 is being played whereas a FFA map knows the exact number of players.
If, for example, a 3v1 is played a team mode map will see it as a 3v3 hence the player on their own still gets 3 player's patches.
