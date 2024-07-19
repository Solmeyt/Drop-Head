# Drop Head
## What's Drop Head ?
**Drop Head** is a project to drop a player's head when they die.

## How it works ?
### Edit player loot table `entities/player.json`
Adds a player head to the death of a player and correlates the characteristics of this dead player

### Add advancement `decapitator.json`
Adds the **Decapitator** advancement which is unlocked by obtaining a player head.

### Add advancement `serialkiller.json`
Adds the **Serial Killer** advancement which is unlocked by killing a player.

### Add advancement `refresh.json` and function `launcher_refresh.mcfunction`
The `refresh.json` advancement launches the `launcher_refresh.mcfunction` function when a player's inventory changes.
The `launcher_refresh.mcfunction` launches `refresh.mcfunction` if the player has a player head in his main hand.
`refresh.mcfunction` refreshes the player's head of his main hand and indirectly makes them stackable

## Compatibility
**Drop Head** should work with anything and anywhere.
