---
description: >-
  This page contains the complete list of available commands, including both
  player and administrator commands.
icon: comment
---

# Commands, Permissions & Placeholders

## User Commands (/clan)

{% hint style="success" %}
**Grant them all permissions for user commands**

`runithclans.user.*`
{% endhint %}

<table><thead><tr><th width="251.22216796875">Command</th><th>Description</th><th>Permissions</th></tr></thead><tbody><tr><td><code>create (name) (tag)</code></td><td>Create a new clan.</td><td>runithclans.user.create</td></tr><tr><td><code>invite (accept/deny/player)</code></td><td>Invite a player to your clan.</td><td>runithclans.user.invite</td></tr><tr><td><code>kick (player)</code></td><td>Remove a player from the clan.</td><td>runithclans.user.kick</td></tr><tr><td><code>leave</code></td><td>Leave your current clan.</td><td>runithclans.user.leave</td></tr><tr><td><code>disband</code></td><td>Permanently delete the clan.</td><td>runithclans.user.disband</td></tr><tr><td><code>info (clan)</code></td><td>View information about a clan.</td><td>runithclans.user.info</td></tr><tr><td><code>list (page)</code></td><td>View the list of available clans.</td><td>runithclans.user.list</td></tr><tr><td><code>ally (add/remove/list) (clan)</code></td><td>Manage the clan allies.</td><td>runithclans.user.ally</td></tr><tr><td><code>enemy (add/remove/list) (clan)</code>  </td><td>Manage the clan enemies. </td><td>runithclans.user.enemy</td></tr><tr><td><code>chat (enemy/ally) (enemyClan/allyClan)</code>  </td><td>Toggle clan chat mode.</td><td>runithclans.user.chat</td></tr><tr><td><code>bank (withdraw/deposit) (amount)</code></td><td>Manage the clan bank.</td><td>runithclans.user.bank</td></tr><tr><td><code>base (set)</code></td><td>Manage the clan base.</td><td>runithclans.user.base</td></tr><tr><td><code>rally</code></td><td>Set or teleport to the clan rally point.</td><td>runithclans.user.rally</td></tr><tr><td><code>setrole (player) (role)</code></td><td>Assign a role to a clan member.</td><td>runithclans.user.setrole</td></tr><tr><td><code>rename (name) (tag)</code></td><td>Rename the clan.</td><td>runithclans.user.rename</td></tr><tr><td><code>tag (tag)</code></td><td>Change the clan tag.</td><td>runithclans.user.tag</td></tr><tr><td><code>upgrade</code></td><td>Upgrade the clan.</td><td>runithclans.user.upgrade</td></tr><tr><td><code>friendlyfire</code></td><td>Toggle friendly fire within the clan.</td><td>runithclans.user.friendlyfire</td></tr></tbody></table>

## Admin Commands (/rclan)

{% hint style="success" %}
**Grant them all permissions for admin commands**

`runithclans.admin.*`
{% endhint %}

| Command                                                                                                              | Description                            | Permissions                 |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | --------------------------- |
| `changetag (clan) (newTag)`                                                                                          | Change the tag of any clan.            | runithclans.admin.changetag |
| `chatspy`                                                                                                            | Monitor all clan chat messages.        | runithclans.admin.chatspy   |
| `delete (clan)`                                                                                                      | Force delete any clan.                 | runithclans.admin.delete    |
| `join (clan) (user/mod/co-leader/leader/administrator)`                                                              | Force join into a clan.                | runithclans.admin.join      |
| `stats (set/add/remove/multiply/divide) (amount) (kills/deaths/points/money) (clan/player) (clanName/playerName) -s` | Change statistics for a clan.          | runithclans.admin.stats     |
| `reload`                                                                                                             | Reload the plugin configuration files. | runithclans.admin.reload    |

## Placeholders

<table><thead><tr><th width="374">Placeholder</th><th>Description</th></tr></thead><tbody><tr><td><code>%clan_leaderboard_(kills/deaths/score/points)_(1/2/3/...)%</code>  </td><td>Return clan with the position</td></tr><tr><td><code>%clan_leaderboardpos_(kills/deaths/score/points)%</code>  </td><td>Returns your clan's position on the leaderboard</td></tr></tbody></table>
