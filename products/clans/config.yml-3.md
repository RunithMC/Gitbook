---
icon: file
---

# groups.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
# Permissions
# Ally:
#   ADD_ALLY
#   REMOVE_ALLY
#   HANDLE_ALLY - Accept/deny/cancel
# Enemies:
#   ADD_ENEMY
#   REMOVE_ENEMY
# Bank:
#   DEPOSIT_BANK
#   WITHDRAW_BANK
# Moderation:
#   KICK_PLAYER
#   INVITE_PLAYER
# Administration:
#   DISBAND
#   RENAME
#   SET_BASE
#   SET_ROLE
# Chat:
#   CLAN_CHAT
#   ALLY_CHAT
#   ENEMY_CHAT
# Others:
#   MODIFY_FRIENDLY_FIRE
#   CHANGE_TAG
#   RALLY
#   UPGRADE
USER:
  permissions:
    - DEPOSIT_BANK
    - CLAN_CHAT
    - ALLY_CHAT
    - ENEMY_CHAT
    - RALLY

MOD:
  extends: USER
  permissions:
    - INVITE_PLAYER
    - KICK_PLAYER

CO_LEADER:
  extends: MOD
  permissions:
    - ADD_ALLY
    - REMOVE_ALLY
    - HANDLE_ALLY
    - ADD_ENEMY
    - REMOVE_ENEMY
    - RENAME
    - SET_BASE
    - MODIFY_FRIENDLY_FIRE
    - CHANGE_TAG
    - UPGRADE
    - SET_ROLE

LEADER:
  extends: CO_LEADER
  permissions:
    - WITHDRAW_BANK
    - DISBAND
```
{% endcode %}
