---
icon: head-side-speak
---

# en\_US.yml

```yaml
aliases:
  - "en_UD"
  - "en_PT"
  - "en_NZ"
  - "en_GB"
  - "en_CA"
  - "en_AU"

messages:
  action-dont-registered: "&8» &cThis action is not registered. Contact an administrator."
  in-process: "&8» &cWait for the task to finish: %action% for clan %clan%"
  roles:
    ADMINISTRATOR: "&4&lADMIN"
    LEADER: "&b&lLEADER"
    CO_LEADER: "&3&lCO_LEADER"
    MOD: "&9&lMOD"
    USER: "&5&lUSER"

  role-error-message:
    ADD_ALLY: "&8» &cYou need to be at least &eCO_LEADER &cto create an alliance."
    REMOVE_ALLY: "&8» &cYou need to be at least &eCO_LEADER &cto remove an alliance."
    HANDLE_ALLY: "&8» &cYou need to be at least &eCO_LEADER &cto accept/deny/cancel an alliance."
    ADD_ENEMY: "&8» &cYou need to be at least &eCO_LEADER &cto add an enemy clan."
    REMOVE_ENEMY: "&8» &cYou need to be at least &eCO_LEADER &cto remove an enemy clan."
    DEPOSIT_BANK: "&8» &cYou need to be at least &eUSER &cto deposit money into the clan bank."
    WITHDRAW_BANK: "&8» &cYou need to be at least &eLEADER &cto withdraw money from the clan bank."
    KICK_PLAYER: "&8» &cYou need to be at least &eMOD &cto kick players from the clan."
    INVITE_PLAYER: "&8» &cYou need to be at least &eMOD &cto invite players to the clan."
    DISBAND: "&8» &cYou need to be at least &eLEADER &cto disband the clan."
    RENAME: "&8» &cYou need to be at least &eCO_LEADER &cto rename the clan."
    SET_BASE: "&8» &cYou need to be at least &eCO_LEADER &cto set the clan base."
    CLAN_CHAT: "&8» &cYou need to be at least &eUSER &cto use clan chat."
    ALLY_CHAT: "&8» &cYou need to be at least &eUSER &cto use ally chat."
    ENEMY_CHAT: "&8» &cYou need to be at least &eUSER &cto use enemy chat."
    MODIFY_FRIENDLY_FIRE: "&8» &cYou need to be at least &eCO_LEADER &cto modify friendly fire."
    CHANGE_TAG: "&8» &cYou need to be at least &eCO_LEADER &cto change the clan tag."
    RALLY: "&8» &cYou need to be at least &eUSER &cto call a rally."
    UPGRADE: "&8» &cYou need to be at least &eCO_LEADER &cto upgrade the clan."
    SET_ROLE: "&8» &cYou need to be at least &eCO_LEADER &cto change role to another player."

  permission-errors:
    USER_UPGRADE: "&8» &cYou do not have permission to upgrade your clan."
    USER_TAG: "&8» &cYou do not have permission to change your clan's tag."
    USER_SETROLE: "&8» &cYou do not have permission to change members' roles."
    USER_RENAME: "&8» &cYou do not have permission to rename your clan."
    USER_RALLY: "&8» &cYou do not have permission to call a rally."
    USER_LIST: "&8» &cYou do not have permission to view the clan list."
    USER_LEAVE: "&8» &cYou do not have permission to leave your clan."
    USER_KICK: "&8» &cYou do not have permission to kick members from your clan."
    USER_INVITE: "&8» &cYou do not have permission to manage clan invitations."
    USER_INFO: "&8» &cYou do not have permission to view clan information."
    USER_FRIENDLYFIRE: "&8» &cYou do not have permission to manage friendly fire settings."
    USER_ENEMY: "&8» &cYou do not have permission to manage enemies."
    USER_DISBAND: "&8» &cYou do not have permission to disband your clan."
    USER_CREATE: "&8» &cYou do not have permission to create a clan."
    USER_CHAT: "&8» &cYou do not have permission to use clan chat features."
    USER_BASE: "&8» &cYou do not have permission to manage your clan's base."
    USER_BANK: "&8» &cYou do not have permission to manage the clan bank."
    USER_ALLY: "&8» &cYou do not have permission to manage alliances."
    USER_USE: "&8» &cYou do not have permission to use clan commands."

  format:
    - "&3&lRunithClans" # You can use hex colors, example: #AFCF21
    - " "
    - "&fAvailable Commands &7→"
    - " &8● &bcreate &9(name) (tag) &8- &fCreate a clan"
    - " &8● &bdisband &8- &fDelete your clan"
    - " &8● &bleave &8- &fLeave your clan"
    - " &8● &bkick &9(player) &8- &fKick a player"
    - " &8● &btag &9(new) &8- &fChange the clan tag"
    - " &8● &blist &9(page) &8- &fShow connected clans"
    - " &8● &binfo &9(clan) &8- &fShow clan information"
    - " &8● &bchat &9(enemy) (enemy clan) &8- &fToggle between chats"
    - " &8● &binvite &9(accept/deny/player) &8- &fManage invitations"
    - " &8● &bsetrole &9(player) (role) &8- &fChange a member's role"
    - " &8● &bbank &9(withdraw/deposit) (amount) &8- &fManage clan bank"
    - " &8● &bally &9(add/remove/list) (name) &8- &fManage alliances"
    - " &8● &benemy &9(add/remove) (name) &8- &fManage enemies"
    - " &8● &bupgrades &8- &fPurchase clan upgrades"
    - " &8● &bbase &9(set) &8- &fGo to/change clan base"
    - " &8● &brally &8- &fSummon all your members"
    - " &8● &bfriendlyfire &8- &fEnable or disable PVP between members"
    - " &8● &brename &9(name) (tag) &8- &fRename the clan"

  create:
    format:
      - "&8» &cUsage: &f/clan create &b(name) (tag)"
      - "&7Example: /clan create &bLosValientes &7(LV)"
    no-in-clan: "&8» &cYou do not belong to any clan."
    already_exist: "&8» &cThe clan &b%clan% &calready exists."
    already_in_clan: "&8» &cYou are already in a clan. Use &b/clan leave &cto leave before creating another."
    name_to_large: "&8» &cThe clan name cannot exceed &e16 &ccharacters."
    created: "&8» &fYou have created the clan &b%clan% &fwith the tag &b%tag%&f."
    invalid_name: "&8» &cThe name entered is not valid. Only letters, numbers, and some symbols are allowed."

  disband:
    confirm:
      - "&8» &cUse &f/clan disband &4&lconfirm &cto confirm."
      - "&e⚠ &6This action is permanent and will delete all clan statistics."
      - "&7If you only wish to transfer leadership, use &b/clan setrole (player) leader&7."
    no-in-clan: "&8» &cYou do not belong to any clan."
    info-to-members: "&8» &6Your clan has been disbanded by leader &b%leader%&6."

  leave:
    is-leader: "&8» &cYou cannot leave the clan as the leader. Use &b/clan disband &cor transfer leadership."
    successfully: "&8» &fYou have left the clan."
    info-to-members: "&8» &ePlayer &b%player% &ehas left the clan."
    no-in-clan: "&8» &cYou do not belong to any clan."

  tag:
    no-in-clan: "&8» &cYou do not belong to any clan."
    format:
      - "&8» &cUsage: &f/clan tag &b(new_tag)"
      - "&7Example: /clan tag &bLosDuros"
    info-to-members: "&8» &6Player &b%player% &6has changed the clan tag to &b%name%&6."
    invalid:
      - " "
      - "&8» &cThe tag can only contain &eletters&c, &enumbers&c, and valid symbols:"
      - "&7._\\-@#!?$%&*+=:;/\\|^~"
      - "&8» &cLength: &e%tag_length% &c/ &e32 &cmaximum."
      - " "

  list:
    header:
      - " "
      - "&3&lRunithClans &8- &7Connected Clans"
      - " "
    footer:
      - " "
      - "&7Page &b%page% &8/ &b%max_page%"
    item: "&8● &b%clan% &8(&7%online%&f/&7%amount%&8) - &f%tag%"
    back: "&8» &aClick to go back to page &b%page%"
    next: "&8» &aClick to go to page &b%page%"
    no-online: "&8» &cNo connected clans found."

  info:
    format:
      - "&8» &cUsage: &f/clan info &b(name)"
      - "&7Shows clan information, even if it's offline."
    dont-exist: "&8» &cThe clan &b%name% &cdoes not exist."
    header:
      - " "
      - "&7Clan &b%name% &8(&7%online%&f/&7%amount%&8) - &b%tag%"
      - "&8Member | Last Active | Role | Time Since Joining"

    online-player: "&8● &a%name% &8(&aOnline&8) - &b%role% - &8(%time_since_join%)"
    offline-player: "&8● &7%name% &8(&7%last_active%&8) - &b%role%  - &8(%time_since_join%)"

    footer:
      - " "
      - "&8Statistics:"
      - "&8» &fPoints: &b%points% &8| &fKills: &b%kills% &8| &fDeaths: &b%deaths%"
      - "&8» &fMoney: &b%money%"
      - "&8» &fTotal Score: &e%score%"
      - "&8» &fAllies: &b%allies%"
      - "&8» &fEnemies: &b%enemies%"

  friendlyfire:
    on-info-to-members: "&8» &fPlayer &b%player% &fhas &aenabled &fPVP between clan members."
    off-info-to-members: "&8» &fPlayer &b%player% &fhas &cdisabled &fPVP between clan members."
    no-in-clan: "&8» &cYou do not belong to any clan."

  chat:
    format:
      - "&8» &cUsage: &f/clan chat &b(enemy) (enemy clan)"
      - "&8» &cUsage: &f/clan chat &bally (ally clan)"
      - "&7Use only &f/clan chat &7to toggle between global and clan chat."

    global: "&8» &fYou have switched to &bGLOBAL&f chat."
    clan: "&8» &fYou have switched to &bCLAN&f chat."

    enemy: "&8» &fYou can now speak with the enemy clan &b%enemy_tag% &8(&7%enemy%&8)&f."
    enemy-format: "&8» &cUsage: &f/clan chat enemy &b(enemy clan)"
    enemy-offline: "&8» &cThe enemy clan %enemy% is not connected."
    no-found-enemy:
      - "&8» &cEnemy clan &b%enemy%&c not found."
      - "&7Current enemies: &b%enemies%"

    no-in-clan: "&8» &cYou do not belong to any clan."

    ally: "&8» &fYou can now speak with the ally clan &b%ally_tag% &8(&7%ally%&8)&f."
    ally-format: "&8» &cUsage: &f/clan chat ally &b(ally clan)"
    ally-offline: "&8» &cThe ally clan %ally% is not connected."
    no-found-ally:
      - "&8» &cAlly clan &b%ally%&c not found."
      - "&7Current allies: &b%allies%"

  invite:
    format: "&8» &cUsage: &f/clan invite &b(accept/deny/player)"
    target-dont-exist: "&8» &cThe player &b%target% &cis not online."
    yourself: "&8» &cYou cannot invite yourself."
    NO_IN_CLAN: "&8» &cYou do not belong to any clan."
    ALREADY_IN_CLAN: "&8» &cThe player &b%target% &cis already in your clan."
    ALREADY_IN_OTHER_CLAN: "&8» &cThe player &b%target% &calready belongs to clan &b%tag% &8(&7%clan%&8)&c."
    ALREADY_INVITED: "&8» &cYou have already invited this player."
    ALREADY_INVITED_BY_OTHER_CLAN: "&8» &cThe player has already been invited to clan &b%clan%&c."
    NO_INVITED: "&8» &cYou have no pending invitations."
    MAX_MEMBERS: "&8» &cYour clan has reached the limit of &e%max% &cmembers."
    DENIED: "&8» &fYou have &crejected &fthe invitation to clan &b%tag% &8(&7%clan%&8)&f."
    INVITED: "&8» &fYou have been invited to clan &b%tag% &8(&7%clan%&8)&f by &b%sender%&f."
    ACCEPTED: "&8» &fYou have &aaccepted &fthe invitation to clan &b%tag% &8(&7%clan%&8)&f."
    SEND: "&8» &fYou have sent an invitation to &b%target%&f."
    SENDER_QUIT: "&8» &cThe invitation has been cancelled because &b%sender% &cdisconnected."
    EXPIRED: "&8» &cThe invitation to clan &b%tag% &8(&7%clan%&8) &chas expired."
    EXPIRED_SENDER: "&8» &cYour invitation to &b%target% &chas expired."
    info-to-members:
      QUIT: "&8» &ePlayer &b%target% &ehas left; the invitation has expired."
      DENIED: "&8» &ePlayer &b%target% &chas rejected &ejoining the clan."
      INVITED: "&8» &fLeader &b%sender% &fhas invited &b%target%&f."
      ACCEPTED: "&8» &fPlayer &b%target% &fhas &aaccepted &fjoining the clan."
      EXPIRED: "&8» &eThe invitation to &b%target% &ehas expired."

  kick:
    format:
      - "&8» &cUsage: &f/clan kick &b(player) (reason)"
      - "&7Example: /clan kick &bPepito &fInappropriate behavior"
    no-in-clan: "&8» &cYou do not belong to any clan."
    target-dont-exist: "&8» &cThe player &b%target% &cis not in your clan."
    yourself: "&8» &cYou cannot kick yourself. Use &b/clan leave&c."
    high-rank: "&8» &cYou cannot kick someone with a rank equal to or higher than yours."
    info-to-members: "&8» &fPlayer &b%player% &fhas kicked &b%target% &ffor: &e%reason%"
    info-to-kicked: "&8» &cYou have been kicked from the clan by &b%player% &c(reason: &e%reason%&c)."

  set-role:
    format:
      - "&8» &cUsage: &f/clan setrole &b(player) (user/mod/coleader/leader)"
    no-in-clan: "&8» &cYou do not belong to any clan."
    target-dont-exist: "&8» &cThe player &b%target% &cis not in your clan."
    yourself: "&8» &cYou cannot change your own role."
    high-rank: "&8» &cYou cannot modify the role of a player with an equal or higher rank."
    need-high-rank: "&8» &cYou do not have the required rank to perform this action."
    info-to-members: "&8» &fPlayer &b%player% &fhas changed the role of &b%target% &fto &b%target_role%&f."
    change-leader: "&8» &fLeadership was transferred from &b%player% &fto &b%target%&f."
    unexist-role: "&8» &cThe role &b%role% &cdoes not exist. Use: &fuser, mod, coleader, leader."
    same-role: "&8» &cThe player already has that role."
    leader-confirm:
      - "&e&lWARNING: &cuse /clan setrole &6%target% leader &c&lCONFIRM"
      - "&eTo give leadership to another person, automatically afterwards"
      - "&eyou will become a co-leader."

  upgrade:
    no-in-clan: "&8» &cYou do not belong to any clan."
    max-level: "&8» &cThe upgrade &b%upgrade% &chas already reached its maximum level."
    no-enough-balance: "&8» &cYour clan does not have sufficient funds. Requires &e%amount%&c, available: &e%clan_balance%&c."
    info-upgrade: "&8» &fPlayer &b%player% &fupgraded &b%upgrade% &fto level &b%level%&f."

  bank:
    no-in-clan: "&8» &cYou do not belong to any clan."
    format:
      - "&8» &cUsage: &f/clan bank &b(deposit/withdraw) (amount)"
      - "&7Example: /clan bank deposit &b1000"
      - "&7Use only &f/clan bank &7to check the current balance."
    error:
      POSITIVE_OVERFLOW: "&8» &cThe number entered is too large."
      NEGATIVE_OVERFLOW: "&8» &cThe number entered is too low."
      FOUND_SIGN_CHARACTER: "&8» &cDo not include + or - signs in the amount."
      FOUND_INVALID_NUMBER: "&8» &cThe amount &e%amount% &cis not valid."
      EMPTY_STRING: "&8» &cThe amount must be greater than 0."
      cant-withdraw: "&8» &cTransaction error. Could not withdraw the money."
      no-has-enough-money: "&8» &cYou do not have &e%amount% &cto deposit."
      clan-no-has-enough-money: "&8» &cThe clan does not have enough funds (&b%clan_amount%&c)."
    info: "&8» &fClan balance: &b%amount%"
    successfully:
      deposit: "&8» &fPlayer &b%player% &fdeposited &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."
      withdraw: "&8» &fPlayer &b%player% &fwithdrew &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."

  enemy:
    format:
      - "&8» &cUsage: &f/clan enemy &b(add/remove) (name)"
      - "&7Example: /clan enemy add &bClanDePepe"
    no-in-clan: "&8» &cYou do not belong to any clan."
    max-enemies: "&8» &cYour clan has reached the limit of &e%max% &cenemies."
    no-online: "&8» &cYou can only declare an enemy to a connected clan."
    add: "&8» &fPlayer &b%player% &fhas declared the clan &b%enemy_tag% &8(&7%enemy_name%&8)&f as an enemy."
    remove: "&8» &fPlayer &b%player% &fhas removed the clan &b%enemy% &ffrom the enemy list."
    cant-remove: "&8» &cThe clan &b%enemy% &cis not on your enemy list."
    same-clan: "&8» &cYou cannot add your own clan as an enemy."

  ally:
    format: "&8» &cUsage: &f/clan ally &b<add|remove|accept|deny|cancel|list> (clan)"
    add-format: "&8» &cUsage: &f/clan ally add &b(clan)"
    accept-format: "&8» &cUsage: &f/clan ally accept &b(clan)"
    deny-format: "&8» &cUsage: &f/clan ally deny &b(clan)"
    cancel-format: "&8» &cUsage: &f/clan ally cancel &b(clan)"
    remove-format: "&8» &cUsage: &f/clan ally remove &b(clan)"
    no-in-clan: "&8» &cYou do not belong to any clan."
    clan-not-found: "&8» &cThe clan &b%clan% &cwas not found."
    cannot-ally-yourself: "&8» &cYou cannot form an alliance with your own clan."
    already-allied: "&8» &cYou are already allied with &b%clan%&c."
    cannot-ally-enemy: "&8» &cYou cannot have an alliance with &b%clan% &cbecause they are your enemy."
    max-allies: "&8» &cYou cannot have more than &b%max% &calliances."
    target-max-allies: "&8» &cThe clan &b%clan% &calready has the maximum number of alliances."
    not-allied: "&8» &cYou are not allied with &b%clan%&c."
    no-pending-request: "&8» &cThere is no pending alliance request with &b%clan%&c."
    no-permission: "&8» &cYou do not have permission to manage alliances."

    request-sent: "&8» &aAlliance request sent to &b%clan%&a."
    request-received: "&8» &b%clan% &arequests an alliance with you &8(&7sent by &b%sender%&8)"
    already-pending-request: "&8» &cThere is already a pending alliance request with %clan%"
    accepted: "&8» &aYou have accepted the alliance with &b%clan%&a."
    denied: "&8» &cYou have rejected the alliance with &b%clan%&c."
    cancelled: "&8» &cYou have cancelled the alliance request with &b%clan%&c."
    removed: "&8» &aYou have broken the alliance with &b%clan%&a."

    request-denied: "&8» &cThe clan &b%clan% &chas rejected your alliance request."
    request-cancelled: "&8» &cThe clan &b%clan% &chas cancelled their alliance request."
    added-broadcast: "&8» &a¡Your clan has allied with &b%clan%&a!"
    removed-broadcast: "&8» &cYour clan has broken the alliance with &b%clan%&c."
    clan-disbanded: "&8» &cYour clan has broken the alliance with &b%clan% &cas it was deleted."

    no-allies: "&8» &cYour clan has no alliances."
    header:
      - " "
      - "&8&l» &7Your Clan's Alliances"
      - ""
    entry: "&8● &7%clan% &8(&7%online%&8/&7%total%&8)"

    cannot-damage: "&8» &cYou cannot attack members of &b%clan% &cbecause they are allies."

  rally:
    no-in-clan: "&8» &cYou do not belong to any clan."
    info-to-members: "&3[RALLY] &fPlayer &a%player% &frequests support at &a%worldguard_region_name%&f."
    expired-info-to-members: "&4⚠ &cThe rally has expired."
    expired-info-to-ally: "&4⚠ &cThe rally from clan %clan% has expired."
    info-to-ally: "&3[RALLY] &fPlayer &a%player% &ffrom clan &b%clan% &frequests support at &a%worldguard_region_name%&f."

  base:
    no-in-clan: "&8» &cYou do not belong to any clan."
    info-to-members: "&3[BASE] &fPlayer &a%player% &fhas changed the base to &e%x%, %y%, %z%."
    in-blacklisted-world: "&8» &cYou are in a blacklisted world, you cannot go to/change the base."
    no-exists: "&8» &cYour clan does not have a base set."
    teleport: "&8» &aYou have been sent to the clan base."
    format: "&8» &cTo set your clan's base, use: /clan base set."

  rename:
    no-in-clan: "&8» &cYou do not belong to any clan."
    already-exists: "&8» &cA clan with this name already exists"
    info-to-members: "&3[RENAME] &fPlayer &a%player% &fhas changed the clan name to %clan% with the tag %tag%&f."
    format: "&8» &cTo rename your clan, use: /clan rename (name) (tag)."

    already_exist: "&8» &cThe clan &b%clan% &calready exists."
    already_in_clan: "&8» &cYou are already in a clan. Use &b/clan leave &cto leave before creating another."
    name_to_large: "&8» &cThe clan name cannot exceed &e16 &ccharacters."
    renamed: "&8» &fYou have renamed the clan to &b%clan% &fwith the tag &b%tag%&f."
    invalid_name: "&8» &cThe name entered is not valid. Only letters, numbers, and some symbols are allowed."
    cooldown: "&8» &cYou need to wait &e%time% &cbefore renaming the clan back"
```
