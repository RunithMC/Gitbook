---
icon: file
---

# example\_crate.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
id: Test
display-name: '&7Test'
require-empty-inventory-to-open: false

# If this is in false, only 1 reward is given and win-commands is executed once, 1#() will be changed to amount,
# else with iterate every reward until reach 0 keys (1#()) is keep in 1.
massive-opening-loop: false

crate-gui:
  id: "D"
  type: "CHEST"
  name: "&cCrate Example"
  papi-parser: true
  lore:
    - "&8Open your keys"
    - ""
    - " &8❙ &fUse your virtual keys"
    - " &8❙ &fto open the crate."
    - ""
    - "&8● &fTest Keys: &6%crates_Test%"
    - ""
    - "  &a◄ Left click to open ►"
    - "  &c► Right click to preview ►"
    - "  &a◄ Shift + click to open all ►"

rewards:
  '0': # Unique identifier for the reward
    display-item:
      amount: 1 # Amount of the item
      type: DOUBLE_PLANT # Item type (must be valid Minecraft material)
      lore: # Example lore
        - '§7+200 tokens'
      flags:
        - "HIDE_ENCHANTS"
        - "HIDE_ATTRIBUTES"
    win-commands:
      - "eco add 1#(200) tokens %player%" # Command to execute when this reward is won
      - "broadcast &6[Crates] &e%player% &awon &6 1#(200) tokens at crate &7Test"
    probability: 50.0
  '1':
    display-item:
      amount: 1
      type: PAPER
      lore:
        - '§7+500 money'
      flags:
        - "HIDE_ENCHANTS"
        - "HIDE_ATTRIBUTES"
    win-commands:
      - "eco add 1#(500) money %player%"
      - "broadcast &6[Crates] &e%player% &awon &6 1#(500) money at crate &7Test"
    probability: 50.0
```
{% endcode %}
