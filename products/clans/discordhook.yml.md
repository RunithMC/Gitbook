---
icon: file
---

# discordhook.yml

{% code overflow="wrap" fullWidth="false" %}
```yml
date-format: 'dd/MM/yyyy HH:mm:ss'
# See https://docs.oracle.com/javase/8/docs/api/java/time/format/DateTimeFormatter.html for more info on date formats

# Placeholders:
# %name%            -> Clan name
# %tag%             -> Clan tag (formatted)
# %members%         -> Comma-separated list of clan members
# %members_count%   -> Total amount of clan members
# %kills%           -> Total clan kills
# %deaths%          -> Total clan deaths
# %points%          -> Clan points
# %balance%         -> Clan balance
# %date%            -> Formatted date (see date-format below)
#
# Event-specific placeholders may also be available depending on the message

create:
  webhook-url: '' # See https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks for how to get this URL
  title: '🏰 CLAN CREATED'
  #disable: true # Uncomment this line to disable this message
  description:
    - ':crown: **Clan:** %name%'
    - ':crossed_swords: **Tag:** `%tag%`'
    - ':bust_in_silhouette: **Leader:** %leader%'
    - ':calendar: **Date:** %date%'

disband:
  webhook-url: ''
  title: '💔 CLAN DISBANDED'
  description:
    - ':crown: **Clan:** %name%'
    - ':crossed_swords: **Tag:** `%tag%`'
    - ':bar_chart: **Members:** %members%' # Support %members_count%
    - ':calendar: **Date:** %date%'

leave:
  webhook-url: ''
  title: '🚪 CLAN LEAVE'
  description:
    - ':crown: **Clan:** %name%'
    - ':bust_in_silhouette: **Player:** %player%'
    - ':calendar: **Date:** %date%'

join:
  webhook-url: ''
  title: '👤 CLAN JOIN'
  description:
    - ':crown: **Clan:** %name%'
    - ':bust_in_silhouette: **Player:** %player%'
    - ':calendar: **Date:** %date%'

enemy-added:
  webhook-url: ''
  title: '⚔️ CLAN ENEMY ADDED'
  description:
    - ':crown: **Clan:** %clan% x %enemy%'
    - ':calendar: **Date:** %date%'

enemy-removed:
  webhook-url: ''
  title: '🛡️ CLAN ENEMY REMOVED'
  description:
    - ':crown: **Clan:** %clan% x %enemy%'
    - ':calendar: **Date:** %date%'

ally-added:
  webhook-url: ''
  title: '🤝 CLAN ALLY ADDED'
  description:
    - ':crown: **Clan:** %clan% x %ally%'
    - ':calendar: **Date:** %date%'

ally-removed:
  webhook-url: ''
  title: '🛡️ CLAN ALLY REMOVED'
  description:
    - ':crown: **Clan:** %clan% x %ally%%'
    - ':calendar: **Date:** %date%'

kick:
  webhook-url: ''
  title: '👢 CLAN KICK'
  description:
    - ':crown: **Clan:** %name%'
    - ':bust_in_silhouette: **Player:** %player% by %kicker%'
    - ':bar_chart: **Reason:** %reason%'
    - ':calendar: **Date:** %date%'

rename:
  webhook-url: ''
  title: '✏️ CLAN RENAMED'
  description:
    - ':crown: **Clan:** %old_name% x %new_name%'
    - ':crossed_swords: **Tag:** `%tag%`'
    - ':calendar: **Date:** %date%'
```
{% endcode %}
