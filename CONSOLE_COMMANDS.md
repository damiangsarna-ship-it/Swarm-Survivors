# Developer Console Commands

The developer console can be opened by pressing the backtick (`) key while the game is running. It provides a powerful set of commands for debugging, testing, and content creation.

---

## Command List

### 1. `give`
Adds items, stats, or currency to the player.

**Usage:** `give <type> <name> [value]`

| Type | Name | Value (Optional) | Description |
| :--- | :--- | :--- | :--- |
| `item` | `<ItemID>` | `[amount]` | Adds a weapon or passive item. If the player already has it, increases its level by `amount`. Defaults to 1. |
| `coins`| `<amount>` | - | Adds the specified `amount` of coins. |
| `xp` | `<amount>` | - | Grants the player the specified `amount` of experience points. |
| `stat` | `<StatName>` | `<amount>` | Increases the specified player stat by `amount`. |
| `pick_up`| `<PickupID>`| - | Spawns and instantly collects the specified pickup item. |

**Examples:**
- `give item wand 3` - Gives a level 3 Wand.
- `give coins 5000` - Adds 5000 coins.
- `give xp 100` - Grants 100 XP.
- `give stat Might 50` - Increases Might by 50.
- `give pick_up chest` - Spawns and opens a chest.

---

### 2. `set`
Sets a game or player value to a specific amount.

**Usage:** `set <type> <name> <value>`

| Type | Name | Value | Description |
| :--- | :--- | :--- | :--- |
| `time` | `<minutes>` | `<seconds>` | Sets the in-game timer to the specified time. |
| `stat` | `<StatName>`| `<value>` | Sets the specified player stat to an exact `value`. |

**Notes on Stat Names:** For stats with spaces (e.g., "Max Health"), remove the space for the command (`MaxHealth`).

**Examples:**
- `set time 15 30` - Sets the game clock to 15:30.
- `set stat MaxHealth 250` - Sets the player's maximum health to 250.

---

### 3. `spawn`
Spawns an entity near the player.

**Usage:** `spawn <name> [amount]`

| Name | Amount (Optional) | Description |
| :--- | :--- | :--- |
| `<EnemyID>` | `[count]` | Spawns the specified number of a given enemy type. Defaults to 1. |
| `<PickupID>`| `[count]` | Spawns the specified number of a given pickup. Defaults to 1. |

**Examples:**
- `spawn goblin 20` - Spawns 20 Goblins.
- `spawn chest 3` - Spawns 3 chests.

---

### 4. `help`
Displays a list of all available commands or provides details on a specific one.

**Usage:** `help [command_name]`

| Command Name (Optional) | Description |
| :--- | :--- |
| - | Lists all available commands. |
| `<CommandName>` | Shows the detailed usage and description for the specified command. |

**Examples:**
- `help`
- `help give`

---

### 5. `clear`
Clears all text from the console output.

**Usage:** `clear`
