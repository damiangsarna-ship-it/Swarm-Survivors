# Developer Console Commands

The developer console can be opened by pressing the backtick (`) key.

## `give <type> <name> [value]`

Gives the player items, currency, or stats.

**Arguments:**

-   `type`: The type of item to give. Can be `item`, `coins`, `xp`, or `stat`.
-   `name`: The name of the item, or the stat to modify.
-   `value` (optional): The amount to give, or the level to set. Defaults to `1`.

**Examples:**

-   `give item wand`: Gives the player a level 1 Wand.
-   `give item iron_plate 3`: Gives the player 3 levels of Iron Plate.
-   `give coins 1000`: Adds 1000 coins to the player's inventory.
-   `give xp 500`: Adds 500 XP to the player.
-   `give stat Might 25`: Increases the player's Might stat by 25.

---

## `set <type> <name> <value>`

Sets a game value or player stat to a specific value.

**Arguments:**

-   `type`: The type of value to set. Can be `time` or `stat`.
-   `name`: The name of the stat to set.
-   `value`: The value to set.

**Examples:**

-   `set time 5 30`: Sets the game time to 5 minutes and 30 seconds.
-   `set stat "Move Speed" 300`: Sets the player's Move Speed to 300.

---

## `spawn <itemName> [amount]`

Spawns enemies or pickups near the player.

**Arguments:**

-   `itemName`: The name of the enemy or pickup to spawn.
-   `amount` (optional): The number of items to spawn. Defaults to `1`.

**Examples:**

-   `spawn goblin 10`: Spawns 10 goblins near the player.
-   `spawn chest`: Spawns a chest near the player.

---

## `give_pickup <name>`

Spawns and instantly collects a pickup item.

**Arguments:**

-   `name`: The name of the pickup to collect.

**Examples:**

-   `give_pickup floor_chicken`: Instantly collects a floor chicken, healing the player.
-   `give_pickup clock`: Instantly collects a clock, freezing all enemies.

---

## `help [command]`

Shows a list of commands or help for a specific command.

**Arguments:**

-   `command` (optional): The command to get help for.

**Examples:**

-   `help`: Lists all available commands.
-   `help give`: Shows detailed help for the `give` command.

---

## `clear`

Clears the console output.
