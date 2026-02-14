---
description: >-
  Learn how to create a custom trade category from scratch with this complete
  step-by-step guide.
icon: file
---

# How to Create a Trade Category

***

### Step 1: Basic Category Configuration

Start by defining your category’s basic information:

```yaml
id: ExampleCategory        # Unique identifier for the category
layout-char: 'E'           # Character used in main config layout
```

#### Explanation:

* **id:** Unique internal ID for the category. Used to link layouts and references.
* **layout-char:** This character connects the category to the main menu layout (config.yml).

***

### Step 2: Configure the Category Display (Main Menu Icon)

This is the icon players see in the main Trades menu.

```yaml
main-display:
  id: "B"
  type: "SKULL_ITEM"
  skull-texture: "BASE64_TEXTURE"
  name: "&fSwords"
  papi-parser: true
  lore:
    - "&8Trade sponges for swords."
    - ""
    - "  &d◄ Click to view ►"
```

#### Explanation:

* **id:** Reference ID used internally (not the layout character).
* **type:** Minecraft material (can be any valid material).
* **skull-texture:** Base64 texture for custom heads.
* **name:** Display name with color codes.
* **papi-parser:** Enables PlaceholderAPI support.
* **lore:** Description shown when hovering over the item.

***

### Step 3: Configure the Category Inventory

This is the GUI players see when entering the category.

```yaml
category-inventory:
  title: "  &8Category ExampleCategory "
  layout:
    - "    ?    "
    - "_________"
    - "         "
    - "   0     "
    - "         "
```

#### Explanation:

* **title:** Inventory GUI title.
* **layout:** Visual structure of the inventory.
  * `?` → Info item
  * `_` → Separator
  * `0` → Trade item slot

***

#### Extra Items (Decoration & Info)

```yaml
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
    name: "&8» &7Trade ExampleCategory"
    lore:
      - "&7Get exclusive items."
```

#### Explanation:

* **separator:** Used for visual decoration.
* **info:** Informational item inside the category.

***

### Step 4: Define Trade Items

Now define what players can trade.

```yaml
trade-items:
  '0':
```

Each trade needs a unique identifier (`'0'`, `'1'`, etc.).

***

#### Display Item (What Players Receive)

```yaml
display-item:
  amount: 1
  type: DIAMOND_SWORD
  name: '§8► §fSword §8[§d§k...§8]'
  enchantments:
    DAMAGE_ALL: 1
  lore:
    - ' §8A powerful sword'
    - ''
    - '§b► Enchantments'
    - ' §8● §7Sharpness §d2'
    - ' §8● §7Fire Aspect §32'
    - ' §8● §7Unbreaking §33'
  flags:
    - "HIDE_ENCHANTS"
    - "HIDE_ATTRIBUTES"
```

#### Explanation:

* **type:** Minecraft material.
* **amount:** Quantity given.
* **enchantments:** Vanilla enchantments.
* **flags:** Hides default attributes and enchant glow.

***

#### Required Items (What Player Must Give)

```yaml
required-items:
  '0':
    type: "GOLD_NUGGET"
    amount: 1
    extra-nbt: |
      {RunithItems:"star"}
```

#### Explanation:

* **type:** Required item material.
* **amount:** Required quantity.
* **extra-nbt:** Custom NBT validation (**Optional**).

***

#### Trade Commands (Reward Execution)

```yaml
trade-commands:
  - "ritems give swordUniverse %player% %amount%"
```

#### Explanation:

* Commands executed after a successful trade.
* `%player%` automatically replaces with player name.
* `%amount%` replaces with traded quantity (for mass trades).

***

### Step 5: Connect the Category to config.yml

To make the category appear in the main Trades menu, edit your `config.yml`.

```yaml
main-inventory:
  title: "  &8Trades Menu "
  layout:
    - "    ?    "
    - "_________"
    - "         "
    - "   E     "
    - "         "
```

#### Explanation:

* The character **E** matches `layout-char: 'E'` in the category file.
* This is how the system links the category to the main menu.
