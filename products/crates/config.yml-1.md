---
icon: file
---

# config.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
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

preview-inventory:
  title: "  &8Preview | %id% "
  layout: # Empty slots will be filled with reward items
    - "_________"
    - "_       _"
    - "_       _"
    - "_       _"
    - "_       _"
    - "<_______>"

  back:
    id: '<'
    type: "ARROW"
    name: "&cBack"

  next:
    id: '>'
    type: "DOUBLE_PLANT"
    name: "&eNext page"

  filler:
    id: "_"
    type: "STAINED_GLASS_PANE"
    data: 15
    name: " "

# extra-items:
#   other:
#     id: "?"
#     type: "STAINED_GLASS_PANE"
#     data: 7
#     name: " "
```
{% endcode %}
