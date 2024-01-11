# Fan The Hammer 2
A Unity3D project developed by Jaren (sigani) with the intention of learning unity, ASP.net, and developing a classic childhood game (at least my childhood).

## About
This is based off of a game that I played with my friends on the playground.  It didn't have an official name, but I heard it being called "James Bond" or "War Game".  
I added my twist to this game and named it "Fan The Hammer" because of the nature of the original game, it was possible to deadlock the game (repeatedly dodge) and so I wanted to add a mechanic to punish players who do so.

## Rules
- Round based game: both players decide on an action to take at the same time.
- Lives: 4
- Starting Ammo: 0
- Max Ammo Count: 6
- Each player decides between 4 options: Reload, Fire, Dodge, Fan The Hammer
  - Reload: loads a bullet into the gun
    - Loses to Fire, Fan The Hammer
  - Fire: fires a bullet at the enemy
    - Costs: 1 bullet
    - Beats: Reload
    - Ties to: Fire (both bullets are wasted)
    - Loses to Fan The Hammer
    - Deals 1 damage if successful
  - Dodge: attempts to dodge a bullet
    - Beats: Fire (doesn't take damage)
    - Loses to Fan The Hammer
  - Fan The Hammer: unloads the entire clip into their opponent
    - Costs: 6 bullets 
    - Beats: Reload, Fire, Dodge
    - Ties against: Fan The Hammer
    - Deals 1 damage if successful
- Upon taking damage, both player's ammo count resets to 0
- The first person to successfully damage their opponent 4 times wins!

## Future Goals
After developing the MVP and refining the textures, I plan on adding additional items and multiplayer functionality.
Example items such as:
- Hollow bullets (deals 2 damage when successful but loses to normal bullets/fires)
- Whiskey (spend 1 bullet, skip a turn, heal 1 life)
