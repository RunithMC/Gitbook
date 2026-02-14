---
icon: file
---

# upgrades.yml

{% code overflow="wrap" %}
```yml
# Clarifications:
# The cost increase “ADD” is the sum of all prices from the previous levels. Let's assume that level 1 is worth 20k, level 2 would be worth 20k,
# level 3 would be worth 60k, level 4 would be worth 80k, and so on.
#
# The MULTIPLY type defines a progressive multiplicative increase in cost per level.
# Each level costs a higher percentage than the previous one, determined by the multiply-factor.
# Basic formula: Cost of level N = value × (multiply-factor ^ N)
#
# STATIC is always a constant value, regardless of the level. It will always be the same.
# NONE returns a value of 0 at any level.

# Enables or disables the clan upgrades system.
enable: true

inventory:
  # GUI title shown to players.
  title: "Clan Upgrades"

  # Inventory layout design.
  # Each character represents a slot item ID.
  layout:
    - "    ?"
    - "_________"
    - " D R M E "
    - ""

  extra-items:
    # Decorative separator item.
    separator:
      id: "_"
      type: "STAINED_GLASS_PANE"
      data: 15
      name: " "

    # Information item explaining how the system works.
    info:
      id: "?"
      type: "BOOK"
      # papi-parser: true (Enable if using PlaceholderAPI parsing)
      name: "&6What is this about?"
      lore:
        - "&fDepending on the clan's money,"
        - "&fthey can upgrade things like: &cextra damage&f,"
        - "&7resistance&f and &etotal member capacity"

# =====================================================
# Extra Damage Upgrade
# =====================================================

extra-damage:
  enable: true

  # Maximum upgrade level.
  max-level: 50

  # Percentage bonus gained per level.
  percentage-per-level: 0.1

  # Base percentage before upgrades.
  base-percentage: 0

  # Cost scaling configuration.
  cost-increase:
    type: "MULTIPLY" # ADD | MULTIPLY | STATIC | NONE
    multiply-factor: 1.10
    value: 3000

  # GUI Item configuration.
  id: "D"
  type: "IRON_SWORD"
  name: "&cExtra Damage"
  lore:
    - "&8Gain additional damage when attacking"
    - ""
    - "&fLevel: &b%level% &8| &9%max_level%"
    - "&fBonus: &b%current%% &7-> &3%next%%"
    - "&fCost: &3%cost%"
    - ""
    - "&bClick here to upgrade"

# =====================================================
# Extra Resistance Upgrade
# =====================================================

extra-resistance:
  enable: true

  max-level: 50
  percentage-per-level: 0.1
  base-percentage: 0

  cost-increase:
    type: "MULTIPLY" # ADD | MULTIPLY | STATIC | NONE
    multiply-factor: 1.10
    value: 3000

  id: "R"
  type: "DIAMOND_CHESTPLATE"
  name: "&7Extra Resistance"
  lore:
    - "&8Receive reduced damage"
    - ""
    - "&fLevel: &b%level% &8| &9%max_level%"
    - "&fBonus: &b%current%% &7-> &3%next%%"
    - "&fCost: &3%cost%"
    - ""
    - "&bClick here to upgrade"

# =====================================================
# Extra Members Upgrade
# =====================================================

extra-members:
  enable: true

  max-level: 10

  # Additional member slots per level.
  members-per-level: 1

  cost-increase:
    type: "MULTIPLY" # ADD | MULTIPLY | STATIC | NONE
    multiply-factor: 1.10
    value: 3000

  id: "M"
  type: "REDSTONE_BLOCK"
  name: "&6Extra Members"
  lore:
    - "&8Increase the maximum clan member capacity"
    - ""
    - "&fLevel: &b%level% &8| &9%max_level%"
    - "&fBonus: &b+%current% &7-> &3%next%"
    - "&fCost: &3%cost%"
    - ""
    - "&bClick here to upgrade"

# =====================================================
# Extra Kill Per Enemy Upgrade
# =====================================================

extra-kill-per-enemy:
  enable: true

  max-level: 25

  # Probability increase per level (percentage).
  probability-per-level: 1

  # Base probability before upgrades.
  base-probability: 0

  cost-increase:
    type: "MULTIPLY" # ADD | MULTIPLY | STATIC | NONE
    multiply-factor: 1.10
    value: 3000

  id: "E"
  type: "SKULL_ITEM"
  name: "&3Extra Kills Per Enemy"
  lore:
    - "&8Gain a chance to receive +1 extra clan kill"
    - "&8when killing a player from an enemy clan"
    - "&8(This kill only counts toward clan stats,"
    - "&8not personal statistics)"
    - ""
    - "&fLevel: &b%level% &8| &9%max_level%"
    - "&fChance: &b%current%% &7-> &3%next%%"
    - "&fCost: &3%cost%"
    - ""
    - "&bClick here to upgrade"

```
{% endcode %}
