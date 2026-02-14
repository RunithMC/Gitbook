---
icon: file
---

# config.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
score-weight:
  # Formula used to calculate clan score:
  # (kills * weight) + (deaths * weight) + (points * weight)
  # You can adjust these values to balance competitive ranking.
  kills: 1        # Points added per kill
  deaths: -1      # Points removed per death
  points: 1       # Extra custom points (events, objectives, etc.)

# Time (in seconds) before a clan invitation expires automatically.
invite-expires-in-seconds: 10

rename-cooldown: 1d # Supports time units like s, m, h, d, w

placeholder-top-entry: "&6%clan_name% &8 ► &b%value%"

# Maximum number of members allowed in a clan.
max-members: 16

# Maximum number of enemy clans a clan can have at the same time.
max-enemies: 8

# If enabled, the console will automatically spy on clan chat.
# Can be toggled manually using /rclan chatspy in console.
automatic-enable-console-chat-spy: true

chat-prefix:
  # Prefix format for normal clan chat.
  # Supports color codes (&) and placeholders like %player_name%.
  # If using RunithChat, supports [item] placeholder as well.
  clan: "&6[CLAN] &a%player_name% &8> &e"

  # Format when receiving a message from an enemy clan.
  enemy-receive: "&c[ENEMY &6%enemy% &c-> CLAN] &a%player_name% &8> &e"

  # Format when sending a message to an enemy clan.
  enemy-send: "&3[CLAN->ENEMY &b%enemy%&3] &6%player_name% &8> &e"

# Time (in seconds) before a rally point disappears automatically.
seconds-to-despawn-rally: 30

# Worlds where setting a clan base is not allowed.
base-blacklist-worlds:
  - "world_the_end"
  - "world_nether"
```
{% endcode %}
