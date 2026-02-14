---
icon: layer-group
---

# example\_category.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
id: ExampleCategory
layout-char: 'E'

main-display:
  id: "B"
  type: "SKULL_ITEM"
  skull-texture: "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvZDQ2NzUxNThjMDc2N2VlNTA4YzUyZDUyNDI2Y2VmM2EyYzJiMjliN2U0ODdjOTI5NTNhMzgyM2Y1NjFkMDZhZiJ9fX0="
  name: "&fSwords"
  papi-parser: true
  lore:
    - "&8Trade sponges for swords."
    - ""
    - "  &d◄ Click to view ►"

category-inventory:
  title: "  &8Category ExampleCategory "
  layout:
    - "    ?    "
    - "_________"
    - "         "
    - "   0     "
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
      name: "&8» &7Trade ExampleCategory"
      lore:
        - "&7Get exclusive items."

trade-items:
  '0':
    display-item:
      amount: 1
      type: DIAMOND_SWORD
      name: '§8► §fSword §8[§d§kl§r§5§k;§d§k;§r §c§lU§6§lN§e§lI§a§lV§3§lE§9§lR§5§lS§c§lE §d§kl§r§5§k;§d§k;§r§8]'
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
    required-items:
      '0':
        type: "GOLD_NUGGET"
        amount: 1

        # See SNBT format
        extra-nbt: |
          {RunithItems:"star"}

    trade-commands:
      - "ritems give swordUniverse %player% %amount%"
```
{% endcode %}
