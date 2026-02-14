---
description: >-
  Learn how to create custom crates from scratch with this complete step-by-step
  guide.
icon: question
---

# How to Create a Crate

***

### Step 1: Basic Crate Configuration

Start by defining your crate's basic information:

```yaml
id: Test                    # Unique identifier for the crate (used in commands)
display-name: '&7Test'      # Display name with color codes (&7 = gray)
require-empty-inventory-to-open: false  # Set to true if players need empty inventory
massive-opening-loop: false  # How multiple keys opening behaves
```

**Explanation:**

* `id`: This is used to difference the key from others.
* `display-name`: What players see in messages and GUIs.
* `require-empty-inventory-to-open`: Prevents issues if inventory fills up.
* `massive-opening-loop`: When true, shows each reward individually when opening multiple keys. (Recommended enable it)

***

### Step 2: Configure the Crate GUI

This is the main interface players see when interacting with the crate:

```yaml
crate-gui:
  id: "D"                   # Reference ID used in layout
  type: "CHEST"             # GUI type (CHEST, HOPPER, etc.)
  name: "&cCrate Example"    # GUI title
  papi-parser: true         # Enable PlaceholderAPI support
  lore:                     # Description shown when hovering
    - "&8Open your keys"
    - ""
    - " &8❙ &fUse your virtual keys"
    - " &8❙ &fto open the crate."
    - ""
    - "&8● &fTest Keys: &6%crates_Test%"  # Shows key count
    - ""
    - "  &a◄ Left click to open ►"
    - "  &c► Right click to preview ►"
    - "  &a◄ Shift + click to open all ►"
```

***

### Step 3: Define Rewards

Add the items players can win. Each reward needs a unique identifier:

```yaml
rewards:
  '0':  # First reward
    display-item:           # What players see in preview
      amount: 1
      type: DOUBLE_PLANT    # Minecraft material
      lore:
        - '§7+200 tokens'
      flags:                # Item flags
        - "HIDE_ENCHANTS"
        - "HIDE_ATTRIBUTES"
    
    win-commands:           # Commands executed when winning
      - "eco add 1#(200) tokens %player%"  # 1#(200) = gives 200
      - "broadcast &6[Crates] &e%player% &awon &6 1#(200) tokens at crate &7Test"
    
    probability: 50.0       # Winning chance (total must equal 100%)
  
  '1':  # Second reward
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

**Important Notes:**

* Probabilities must add up to 100%
* Use `1#(amount)` for variable amounts in commands
* `%player%` placeholder automatically replaces with the player's name

***

### Step 4: Design the Main Inventory Layout

Create the visual layout where players can access the crate:

```yaml
main-inventory:
  title: "  &8Crates "
  layout:
    - "    ?    "
    - "_________"
    - "    D    "
    - "         "
  
  extra-items:
    separator:
      id: "_"
      type: "STAINED_GLASS_PANE"
      data: 15
      name: " "

    info:
      id: "?"
      type: "BOOK"
      papi-parser: true
      name: "&8» &7Your Keys"
      lore:
        - "&8Keys Amount"
        - ""
        - " &8❙ &fTest: &6%crates_Test%"
        - ""
```
