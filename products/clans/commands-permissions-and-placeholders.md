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

`runithclans.user.*` or `runithclans.user.use` for /clan usage
{% endhint %}

<table><thead><tr><th width="251.22216796875">Command</th><th>Description</th><th>Permissions</th></tr></thead><tbody><tr><td><code>create (name) (tag)</code></td><td>Create a new clan.</td><td>runithclans.user.create</td></tr><tr><td><code>invite (accept/deny/player)</code></td><td>Invite a player to your clan.</td><td>runithclans.user.invite</td></tr><tr><td><code>kick (player)</code></td><td>Remove a player from the clan.</td><td>runithclans.user.kick</td></tr><tr><td><code>leave</code></td><td>Leave your current clan.</td><td>runithclans.user.leave</td></tr><tr><td><code>disband</code></td><td>Permanently delete the clan.</td><td>runithclans.user.disband</td></tr><tr><td><code>info (clan)</code></td><td>View information about a clan.</td><td>runithclans.user.info</td></tr><tr><td><code>list (page)</code></td><td>View the list of available clans.</td><td>runithclans.user.list</td></tr><tr><td><code>ally (add/remove/list) (clan)</code></td><td>Manage the clan allies.</td><td>runithclans.user.ally</td></tr><tr><td><code>enemy (add/remove/list) (clan)</code></td><td>Manage the clan enemies.</td><td>runithclans.user.enemy</td></tr><tr><td><code>chat (enemy/ally) (enemyClan/allyClan)</code></td><td>Toggle clan chat mode.</td><td>runithclans.user.chat</td></tr><tr><td><code>bank (withdraw/deposit) (amount)</code></td><td>Manage the clan bank.</td><td>runithclans.user.bank</td></tr><tr><td><code>base (set)</code></td><td>Manage the clan base.</td><td>runithclans.user.base</td></tr><tr><td><code>rally</code></td><td>Set or teleport to the clan rally point.</td><td>runithclans.user.rally</td></tr><tr><td><code>setrole (player) (role)</code></td><td>Assign a role to a clan member.</td><td>runithclans.user.setrole</td></tr><tr><td><code>rename (name) (tag)</code></td><td>Rename the clan.</td><td>runithclans.user.rename</td></tr><tr><td><code>tag (tag)</code></td><td>Change the clan tag.</td><td>runithclans.user.tag</td></tr><tr><td><code>upgrade</code></td><td>Upgrade the clan.</td><td>runithclans.user.upgrade</td></tr><tr><td><code>friendlyfire</code></td><td>Toggle friendly fire within the clan.</td><td>runithclans.user.friendlyfire</td></tr></tbody></table>

## Admin Commands (/rclan)

{% hint style="success" %}
**Grant them all permissions for admin commands**

`runithclans.admin.*` or `runithclans.admin.use` for /rclan usage
{% endhint %}

| Command                                                                                                              | Description                                                                          | Permissions                 |
| -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | --------------------------- |
| `changetag (clan) (newTag)`                                                                                          | Change the tag of any clan.                                                          | runithclans.admin.changetag |
| `chatspy`                                                                                                            | Monitor all clan chat messages.                                                      | runithclans.admin.chatspy   |
| `delete (clan)`                                                                                                      | Force delete any clan.                                                               | runithclans.admin.delete    |
| `join (clan) (user/mod/co-leader/leader/administrator)`                                                              | Force join into a clan.                                                              | runithclans.admin.join      |
| `stats (set/add/remove/multiply/divide) (amount) (kills/deaths/points/money) (clan/player) (clanName/playerName) -s` | Change statistics for a clan.                                                        | runithclans.admin.stats     |
| `reload`                                                                                                             | Reload the plugin configuration files.                                               | runithclans.admin.reload    |
| <p><code>migrator (type) (confirm/clean)</code> </p><p></p>                                                          | Migrate from others clan plugins. Support: **simpleclans, advancedclans, clanslite** | runithclans.admin.migrate   |

## Placeholders

If you want get stats from specific clan. Use: %clan\_(clanName):(name/on/tag/...)%

<table><thead><tr><th width="449">Placeholder</th><th>Description</th></tr></thead><tbody><tr><td><code>%clan_leaderboard_(kills/deaths/score/points)_(1/2/3/...)%</code></td><td>Return clan with the position</td></tr><tr><td><code>%clan_leaderboardpos_(kills/deaths/score/points)%</code></td><td>Returns your clan's position on the leaderboard</td></tr><tr><td><code>%clan_name%</code></td><td>Return clan name</td></tr><tr><td><code>%clan_on%</code></td><td>Return amount of players conected</td></tr><tr><td><code>%clan_tag%</code></td><td>Returns your clan's tag</td></tr><tr><td><code>%clan_(kills/deaths/score/money/points)%</code></td><td>Returns your clan's statistics</td></tr><tr><td><code>%clan_chat%</code></td><td>Returns which chat you are in (global, clan, ally, or enemy)</td></tr><tr><td><code>%clan_role%</code></td><td>Returns your rule (user, mod, co-leader, leader or admin)</td></tr><tr><td><code>%clan_jointime%</code></td><td>Returns how long ago you joined the clan, e.g., 2s, 3m, etc.</td></tr><tr><td><code>%clan_lastActiveTime%</code></td><td>Returns how long ago they joined the clan, e.g., 53d, 1y, etc.</td></tr><tr><td><code>%clan_has%</code></td><td>Returns whether the player is in a clan (true/false)</td></tr><tr><td><code>%clan_alliesOn%</code></td><td>Returns the number of allies that are connected</td></tr><tr><td><code>%clan_enemiesOn%</code></td><td>Returns the number of enemies that are connected</td></tr></tbody></table>

## Permissions

<pre class="language-yaml"><code class="lang-yaml"># User permissions
runithclans.user.use: true # Access to /clan
runithclans.user.upgrade: true
runithclans.user.tag: true
runithclans.user.setrole: true
runithclans.user.rename: true
runithclans.user.rally: true
runithclans.user.list: true
runithclans.user.leave: true
runithclans.user.kick: true
runithclans.user.invite: true
runithclans.user.info: true
runithclans.user.friendlyfire: true
runithclans.user.enemy: true
runithclans.user.disband: true
runithclans.user.create: true
runithclans.user.chat: true
runithclans.user.base: true
runithclans.user.bank: true
runithclans.user.ally: true

# Admin permissions
runithclans.admin.<a data-footnote-ref href="#user-content-fn-1">use</a>: true # Access to /rclan 
runithclans.user: true
runithclans.admin.stats: true
runithclans.admin.reload: true
runithclans.admin.join: true
runithclans.admin.delete: true
runithclans.admin.chatspy: true
runithclans.admin.changetag: true
</code></pre>

[^1]: 
