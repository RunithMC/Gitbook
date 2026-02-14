---
description: >-
  This page contains the complete list of available commands, including both
  player and administrator commands.
icon: comment
---

# Commands, Permissions & Placeholders

## User Commands (/crates)

{% hint style="success" %}
**Grant them all permissions for admin commands**

`runithcrates.user.*` or `runithcrates.user.use` for /crates usage
{% endhint %}

<table><thead><tr><th width="251.22216796875">Command</th><th>Description</th><th>Permissions</th></tr></thead><tbody><tr><td><code>crates</code></td><td>Open crate's menu</td><td>runithcrates.user.keys</td></tr></tbody></table>

## Admin Commands (/rcrates)

{% hint style="success" %}
**Grant them all permissions for admin commands**

`runithcrates.admin.*` or `runithcrates.admin.use` for /rcrates usage
{% endhint %}

| Command                                                                  | Description                            | Permissions                      |
| ------------------------------------------------------------------------ | -------------------------------------- | -------------------------------- |
| `keys (set/add/remove/multiply/divide) (amount) (crateName) (player) -s` | Manages a player's keys                | runithcrates.admin.keys          |
| `giveall (amount) (crateName)`                                           | Give keys to everyone                  | runithcrates.admin.giveall       |
| `addlocation`                                                            | Create a crate location to set it      | runithclans.admin.addlocation    |
| `removelocation`                                                         | Delete a crate location to remove it   | runithclans.admin.removelocation |
| `reload`                                                                 | Reload the plugin configuration files. | runithcrates.admin.reload        |

## Placeholders

<table><thead><tr><th width="374">Placeholder</th><th>Description</th></tr></thead><tbody><tr><td><code>%runithcrates_(crateId)_displayName%</code></td><td>Display the crate name</td></tr><tr><td><code>%runithcrates_(crateId)%</code></td><td>Display the player's keys for a crate</td></tr></tbody></table>

