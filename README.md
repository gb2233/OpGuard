<img src="http://i.imgur.com/le8Nqlv.png"></img>

---

OpGuard is a Spigot plugin that protects against op exploits &amp; malicious plugins.

## Config

### Global Section

| Option                           | Description                      |
|----------------------------------|----------------------------------|
| inspection-interval | Amount of time *in ticks* OpGuard should verify the op list. |
| | **Default Value:** `4` *(5 times per second)* |
| save-interval | Amount of time *in ticks* OpGuard should save the config. |
| | **Default Value:** `1200` *(once per minute)* |
| only-op-if-online | If true, OpGuard will only allow online players to gain op. |
| | **Default Value:** `true` |
| shutdown-on-disable | If true, OpGuard will stop the server if another plugin attempts to disable it. |
| | **Default Value:** `false` |

### Log Section

| Option                           | Description                      |
|----------------------------------|----------------------------------|
| enabled | Whether or not logging should occur. |
| | **Default Value:** `true` |
| status | Log status messages. |
| | **Default Value:** `true` |
| plugin-attempt | Log op attempts from other plugins. |
| | **Default Value:** `true` |
| console-attempt | Log op attempts from the console. |
| | **Default Value:** `true` |
| player-attempt | Log op attempts from online players. |
| | **Default Value:** `true` |

### Warn Section

| Option                           | Description                      |
|----------------------------------|----------------------------------|
| status | Recieve notifications about OpGuard's status. |
| | **Default Value:** `true` |
| plugin-attempt | Recieve notifications about op attempts from other plugins. |
| | **Default Value:** `true` |
| console-attempt | Recieve notifications about op attempts from the console. |
| | **Default Value:** `true` |
| player-attempt | Recieve notifications about op attempts from online players. |
| | **Default Value:** `true` |
| security-risk | Recieve security warnings if OpGuard's password isn't set. |
| | **Default Value:** `true` |

### Punish Section

| Option                           | Description                      |
|----------------------------------|----------------------------------|
| plugin-attempt | Punish players from plugin op attempts. |
| | **Default Value:** `true` |
| console-attempt | Punish players from console op attempts. |
| | **Default Value:** `true` |
| player-attempt | Punish players from online player op attempts. |
| | **Default Value:** `false` <br> *Enabling this option is not recommended: innocent players are likely to be punished.* |
| command | The command OpGuard should run to punish players. |
| | **Default Value:** `ban %player% Attempting to gain op` <br> The placeholder **%player%** is replaced with the player attempting to gain op. |

### Password Section

This section shoult **not** be modified manually, but rather with in-game commands. This is where OpGuard stores information about its password; changing even a single character could render the password unusable (assuming it's set).

Only mess with this section if you know what you're doing.

### Verified Section

OpGuard stores verified op users here. This section, like the password section, should **not** be modified manually. All updates to the verified section are done automatically by OpGuard.
