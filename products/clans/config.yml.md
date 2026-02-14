---
icon: file
---

# config.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
score-weight:
  # Formula used to calculate clan score:
  # (kills * weight) + (deaths * weight) + (points * weight) + (balance * weight)
  # You can adjust these values to balance competitive ranking.
  kills: 1        # Points added per kill
  deaths: -1      # Points removed per death
  points: 1       # Extra custom points (events, objectives, etc.)
  balance: 0      # Additional balance factor (can be used to adjust overall scoring)

# Time before a clan invitation expires automatically.
invite-expires-in: 10s # Supports time units like s, m, h, d, y
rename-cooldown: 1d

placeholder-top-entry: "&6%clan_name% &8 ► &b%value%"

# Maximum number of members, enemies, and allies a clan can have.
max-members: 16
max-enemies: 8
max-allies: 3

# If enabled, the console will automatically spy on clan chat.
# Can be toggled manually using /rclan chatspy in console.
automatic-enable-console-chat-spy: true

chat-prefix:
  # Supports color codes (&) and placeholders like %player_name%.
  # If using RunithChat, supports [item] placeholder as well.
  clan: "&6[CLAN] &c%player_name% &8» &e"

  # Format when receiving a message from an enemy clan.
  enemy-receive: "&6[ENEMY] &7(%clan%) &6%player_name% &8» &e"

  # Format when sending a message to an enemy clan.
  enemy-send: "&c[CLAN->ENEMY] &7(%clan%) &6%player_name% &8» &e"

  # Format when receiving a message from an ally clan.
  ally-receive: "&3[ALLY] &7(%clan%) &b%player_name% &8» &e"

  # Format when sending a message to an ally clan.
  ally-send: "&9[CLAN->ALLY] &7(%clan%) &b%player_name% &8» &e"

# Time before a rally point disappears automatically.
cooldown-to-despawn-rally: 30s

# Worlds where setting a clan base is not allowed.
base-blacklist-worlds:
  - "world_the_end"
  - "world_nether"
```
{% endcode %}
