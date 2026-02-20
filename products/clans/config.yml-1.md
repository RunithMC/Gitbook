---
icon: file
---

# chat.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
prefix:
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

# If enabled, the console will automatically spy on clan chat.
# Can be toggled manually using /rclan chatspy in console.
automatic-enable-console-chat-spy: true
```
{% endcode %}
