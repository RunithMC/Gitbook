---
icon: head-side-speak
---

# es\_ES.yml

{% code overflow="wrap" %}
```yml
aliases:
  - "es_ES"
  - "es_AR"
  - "es_CL"
  - "es_MX"
  - "es_CO"
  - "es_PE"

messages:
  action-dont-registered: "&8» &cEsta acción no está registrada. Contacta a un administrador."
  in-process: "&8» &cEspera a que finalice la tarea: %action% para el clan %clan%"
  user-command-no-permission: "&8» &cNo tienes permiso para usar este comando."

  format:
    - "&3&lRunithClans"
    - " "
    - "&fComandos Disponibles &7→"
    - " &8● &bcreate &9(nombre) (tag) &8- &fCrear un clan"
    - " &8● &bdisband &8- &fEliminar tu clan"
    - " &8● &bleave &8- &fAbandonar tu clan"
    - " &8● &bkick &9(jugador) &8- &fExpulsar a un jugador"
    - " &8● &btag &9(nuevo) &8- &fCambiar el tag del clan"
    - " &8● &blist &9(página) &8- &fMostrar clanes conectados"
    - " &8● &binfo &9(clan) &8- &fMostrar información del clan"
    - " &8● &bchat &9(enemy) (clan enemigo) &8- &fCambiar entre chats"
    - " &8● &binvite &9(accept/deny/jugador) &8- &fGestionar invitaciones"
    - " &8● &bsetrole &9(jugador) (rol) &8- &fCambiar el rol de un miembro"
    - " &8● &bbank &9(withdraw/deposit) (cantidad) &8- &fGestionar el banco del clan"
    - " &8● &bally &9(add/remove/list) (nombre) &8- &fGestionar alianzas"
    - " &8● &benemy &9(add/remove) (nombre) &8- &fGestionar enemigos"
    - " &8● &bupgrades &8- &fComprar mejoras para el clan"
    - " &8● &bbase &9(set) &8- &fIr a/cambiar la base del clan"
    - " &8● &brally &8- &fConvocar a todos tus miembros"
    - " &8● &bfriendlyfire &8- &fActivar o desactivar PVP entre miembros"
    - " &8● &brename &9(nombre) (tag) &8- &fRenombrar el clan"

  create:
    format:
      - "&8» &cUso: &f/clan create &b(nombre) (tag)"
      - "&7Ejemplo: /clan create &bLosValientes &7(LV)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    already_exist: "&8» &cEl clan &b%clan% &cya existe."
    already_in_clan: "&8» &cYa estás en un clan. Usa &b/clan leave &cpara salir antes de crear otro."
    name_to_large: "&8» &cEl nombre del clan no puede exceder los &e16 &ccaracteres."
    created: "&8» &fHas creado el clan &b%clan% &fcon el tag &b%tag%&f."
    invalid_name: "&8» &cEl nombre ingresado no es válido. Solo se permiten letras, números y algunos símbolos."

  disband:
    confirm:
      - "&8» &cUsa &f/clan disband &4&lconfirm &cpara confirmar."
      - "&e⚠ &6Esta acción es permanente y eliminará todas las estadísticas del clan."
      - "&7Si solo deseas transferir el liderazgo, usa &b/clan setrole (jugador) leader&7."
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    no-leader: "&8» &cSolo el líder puede eliminar el clan."
    info-to-members: "&8» &6Tu clan ha sido disuelto por el líder &b%leader%&6."

  leave:
    is-leader: "&8» &cNo puedes abandonar el clan siendo el líder. Usa &b/clan disband &co transfiere el liderazgo."
    successfully: "&8» &fHas abandonado el clan."
    info-to-members: "&8» &eEl jugador &b%player% &eha abandonado el clan."
    no-in-clan: "&8» &cNo perteneces a ningún clan."

  tag:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    format:
      - "&8» &cUso: &f/clan tag &b(nuevo_tag)"
      - "&7Ejemplo: /clan tag &bLosDuros"
    no-leader: "&8» &cSolo el líder puede cambiar el tag del clan."
    info-to-members: "&8» &6El jugador &b%player% &6ha cambiado el tag del clan a &b%name%&6."
    invalid:
      - " "
      - "&8» &cEl tag solo puede contener &eletras&c, &enúmeros&c, y símbolos válidos:"
      - "&7._\\-@#!?$%&*+=:;/\\|^~"
      - "&8» &cLongitud: &e%tag_length% &c/ &e32 &cmáximo."
      - " "

  list:
    header:
      - " "
      - "&3&lRunithClans &8- &7Clanes Conectados"
      - " "
    footer:
      - " "
      - "&7Página &b%page% &8/ &b%max_page%"
    item: "&8● &b%clan% &8(&7%online%&f/&7%amount%&8) - &f%tag%"
    back: "&8» &aHaz clic para volver a la página &b%page%"
    next: "&8» &aHaz clic para ir a la página &b%page%"
    no-online: "&8» &cNo se encontraron clanes conectados."

  info:
    format:
      - "&8» &cUso: &f/clan info &b(nombre)"
      - "&7Muestra la información del clan, incluso si está desconectado."
    dont-exist: "&8» &cEl clan &b%name% &cno existe."
    header:
      - " "
      - "&7Clan &b%name% &8(&7%online%&f/&7%amount%&8) - &b%tag%"
      - "&8Miembro | Ultima conexión | Rol | Tiempo en el clan"

    online-player: "&8● &a%name% &8(&aConectado&8) - &b%role% - &8(%time_since_join%)"
    offline-player: "&8● &7%name% &8(&7%last_active%&8) - &b%role%  - &8(%time_since_join%)"

    footer:
      - " "
      - "&8Estadísticas:"
      - "&8» &fPuntos: &b%points% &8| &fAsesinatos: &b%kills% &8| &fMuertes: &b%deaths%"
      - "&8» &fDinero: &b%money%"
      - "&8» &fPuntuación Total: &e%score%"
      - "&8» &fAliados: &b%allies%"
      - "&8» &fEnemigos: &b%enemies%"

  friendlyfire:
    on-info-to-members: "&8» &fEl jugador &b%player% &fha &aactivado &fel PVP entre miembros del clan."
    off-info-to-members: "&8» &fEl jugador &b%player% &fha &cdesactivado &fel PVP entre miembros del clan."
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    need-higher-role: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara cambiar esta configuración."

  chat:
    format:
      - "&8» &cUso: &f/clan chat &b(enemy) (clan enemigo)"
      - "&8» &cUso: &f/clan chat &bally (clan aliado)"
      - "&7Usa solo &f/clan chat &7para alternar entre el chat global y el del clan."

    global: "&8» &fHas cambiado al chat &bGLOBAL&f."
    clan: "&8» &fHas cambiado al chat &bDEL CLAN&f."

    enemy: "&8» &fAhora puedes hablar con el clan enemigo &b%enemy_tag% &8(&7%enemy%&8)&f."
    enemy-format: "&8» &cUso: &f/clan chat enemy &b(clan enemigo)"
    enemy-offline: "&8» &cEl clan enemigo %enemy% no está conectado."
    no-found-enemy:
      - "&8» &cEl clan enemigo &b%enemy%&c no se encontró."
      - "&7Enemigos actuales: &b%enemies%"

    no-in-clan: "&8» &cNo perteneces a ningún clan."

    ally: "&8» &fAhora puedes hablar con el clan aliado &b%ally_tag% &8(&7%ally%&8)&f."
    ally-format: "&8» &cUso: &f/clan chat ally &b(clan aliado)"
    ally-offline: "&8» &cEl clan aliado %ally% no está conectado."
    no-found-ally:
      - "&8» &cEl clan aliado &b%ally%&c no se encontró."
      - "&7Aliados actuales: &b%allies%"

  invite:
    format: "&8» &cUso: &f/clan invite &b(accept/deny/jugador)"
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está conectado."
    yourself: "&8» &cNo puedes auto-invitarte."
    NO_LEADER: "&8» &cSolo el líder puede enviar invitaciones."
    NO_IN_CLAN: "&8» &cNo perteneces a ningún clan."
    ALREADY_IN_CLAN: "&8» &cEl jugador &b%target% &cya está en tu clan."
    ALREADY_IN_OTHER_CLAN: "&8» &cEl jugador &b%target% &cya pertenece al clan &b%tag% &8(&7%clan%&8)&c."
    ALREADY_INVITED: "&8» &cYa has invitado a este jugador."
    ALREADY_INVITED_BY_OTHER_CLAN: "&8» &cEl jugador ya ha sido invitado al clan &b%clan%&c."
    NO_INVITED: "&8» &cNo tienes invitaciones pendientes."
    MAX_MEMBERS: "&8» &cTu clan ha alcanzado el límite de &e%max% &cmiembros."
    DENIED: "&8» &fHas &crechazado &fla invitación al clan &b%tag% &8(&7%clan%&8)&f."
    INVITED: "&8» &fHas sido invitado al clan &b%tag% &8(&7%clan%&8)&f por &b%sender%&f."
    ACCEPTED: "&8» &fHas &aaceptado &fla invitación al clan &b%tag% &8(&7%clan%&8)&f."
    SEND: "&8» &fHas enviado una invitación a &b%target%&f."
    SENDER_QUIT: "&8» &cLa invitación ha sido cancelada porque &b%sender% &cse desconectó."
    EXPIRED: "&8» &cLa invitación al clan &b%tag% &8(&7%clan%&8) &cha expirado."
    EXPIRED_SENDER: "&8» &cTu invitación a &b%target% &cha expirado."
    info-to-members:
      QUIT: "&8» &eEl jugador &b%target% &eha salido; la invitación ha expirado."
      DENIED: "&8» &eEl jugador &b%target% &chas rechazado &eunirse al clan."
      INVITED: "&8» &fEl líder &b%sender% &fha invitado a &b%target%&f."
      ACCEPTED: "&8» &fEl jugador &b%target% &fha &aaceptado &funirse al clan."
      EXPIRED: "&8» &eLa invitación a &b%target% &eha expirado."

  kick:
    format:
      - "&8» &cUso: &f/clan kick &b(jugador) (razón)"
      - "&7Ejemplo: /clan kick &bPepito &fComportamiento inapropiado"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en tu clan."
    yourself: "&8» &cNo puedes expulsarte a ti mismo. Usa &b/clan leave&c."
    high-rank: "&8» &cNo puedes expulsar a alguien con un rango igual o superior al tuyo."
    min-rank: "&8» &cDebes ser al menos &eMOD &cpara expulsar jugadores."
    info-to-members: "&8» &fEl jugador &b%player% &fha expulsado a &b%target% &fpor: &e%reason%"
    info-to-kicked: "&8» &cHas sido expulsado del clan por &b%player% &c(razón: &e%reason%&c)."

  set-role:
    format:
      - "&8» &cUso: &f/clan setrole &b(jugador) (user/mod/coleader/leader)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en tu clan."
    yourself: "&8» &cNo puedes cambiar tu propio rol."
    high-rank: "&8» &cNo puedes modificar el rol de un jugador con rango igual o superior."
    need-high-rank: "&8» &cNo tienes el rango requerido para realizar esta acción."
    min-rank: "&8» &cSolo los &eSUB-LÍDERES &cpueden cambiar roles."
    info-to-members: "&8» &fEl jugador &b%player% &fha cambiado el rol de &b%target% &fa &b%target_role%&f."
    change-leader: "&8» &fEl liderazgo fue transferido de &b%player% &fa &b%target%&f."
    unexist-role: "&8» &cEl rol &b%role% &cno existe. Usa: &fuser, mod, coleader, leader."
    same-role: "&8» &cEl jugador ya tiene ese rol."
    leader-confirm:
      - "&e&lADVERTENCIA: &cusa /clan setrole &6%target% leader &c&lCONFIRM"
      - "&ePara dar el liderazgo a otra persona, automáticamente después"
      - "&ete convertirás en sub-líder."

  upgrade:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    max-level: "&8» &cLa mejora &b%upgrade% &cya ha alcanzado su nivel máximo."
    no-enough-balance: "&8» &cTu clan no tiene fondos suficientes. Requiere &e%amount%&c, disponible: &e%clan_balance%&c."
    info-upgrade: "&8» &fEl jugador &b%player% &fmejoró &b%upgrade% &fal nivel &b%level%&f."

  bank:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    format:
      - "&8» &cUso: &f/clan bank &b(deposit/withdraw) (cantidad)"
      - "&7Ejemplo: /clan bank deposit &b1000"
      - "&7Usa solo &f/clan bank &7para ver el saldo actual."
    error:
      POSITIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado grande."
      NEGATIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado pequeño."
      FOUND_SIGN_CHARACTER: "&8» &cNo incluyas signos + o - en la cantidad."
      FOUND_INVALID_NUMBER: "&8» &cLa cantidad &e%amount% &cno es válida."
      EMPTY_STRING: "&8» &cLa cantidad debe ser mayor a 0."
      cant-withdraw: "&8» &cError en la transacción. No se pudo retirar el dinero."
      no-has-enough-money: "&8» &cNo tienes &e%amount% &cpara depositar."
      clan-no-has-enough-money: "&8» &cEl clan no tiene fondos suficientes (&b%clan_amount%&c)."
    info: "&8» &fSaldo del clan: &b%amount%"
    successfully:
      deposit: "&8» &fEl jugador &b%player% &fdepositó &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."
      withdraw: "&8» &fEl jugador &b%player% &fretiró &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."

  enemy:
    format:
      - "&8» &cUso: &f/clan enemy &b(add/remove) (nombre)"
      - "&7Ejemplo: /clan enemy add &bClanDePepe"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    need-high-rank: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara modificar enemigos."
    max-enemies: "&8» &cTu clan ha alcanzado el límite de &e%max% &cenemigos."
    no-online: "&8» &cSolo puedes declarar enemigo a un clan que esté conectado."
    add: "&8» &fEl jugador &b%player% &fha declarado al clan &b%enemy_tag% &8(&7%enemy_name%&8)&f como enemigo."
    remove: "&8» &fEl jugador &b%player% &fha eliminado al clan &b%enemy% &fde la lista de enemigos."
    cant-remove: "&8» &cEl clan &b%enemy% &cno está en tu lista de enemigos."
    same-clan: "&8» &cNo puedes añadir a tu propio clan como enemigo."

  ally:
    format: "&8» &cUso: &f/clan ally &b<add|remove|accept|deny|cancel|list> (clan)"
    add-format: "&8» &cUso: &f/clan ally add &b(clan)"
    accept-format: "&8» &cUso: &f/clan ally accept &b(clan)"
    deny-format: "&8» &cUso: &f/clan ally deny &b(clan)"
    cancel-format: "&8» &cUso: &f/clan ally cancel &b(clan)"
    remove-format: "&8» &cUso: &f/clan ally remove &b(clan)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    min-rank: "&8» &cNecesitas ser al menos Sub-Líder para gestionar alianzas."
    clan-not-found: "&8» &cEl clan &b%clan% &cno fue encontrado."
    cannot-ally-yourself: "&8» &cNo puedes formar una alianza con tu propio clan."
    already-allied: "&8» &cYa estás aliado con &b%clan%&c."
    cannot-ally-enemy: "&8» &cNo puedes tener una alianza con &b%clan% &cporque son tus enemigos."
    max-allies: "&8» &cNo puedes tener más de &b%max% &calianzas."
    target-max-allies: "&8» &cEl clan &b%clan% &cya tiene el número máximo de alianzas."
    not-allied: "&8» &cNo estás aliado con &b%clan%&c."
    no-pending-request: "&8» &cNo hay ninguna solicitud de alianza pendiente con &b%clan%&c."
    no-permission: "&8» &cNo tienes permiso para gestionar alianzas."

    request-sent: "&8» &aSolicitud de alianza enviada a &b%clan%&a."
    request-received: "&8» &b%clan% &asolicita una alianza contigo &8(&7enviada por &b%sender%&8)"
    already-pending-request: "&8» &cYa hay una solicitud de alianza pendiente con %clan%"
    accepted: "&8» &aHas aceptado la alianza con &b%clan%&a."
    denied: "&8» &cHas rechazado la alianza con &b%clan%&c."
    cancelled: "&8» &cHas cancelado la solicitud de alianza con &b%clan%&c."
    removed: "&8» &aHas roto la alianza con &b%clan%&a."

    request-denied: "&8» &cEl clan &b%clan% &cha rechazado tu solicitud de alianza."
    request-cancelled: "&8» &cEl clan &b%clan% &cha cancelado su solicitud de alianza."
    added-broadcast: "&8» &a¡Tu clan se ha aliado con &b%clan%&a!"
    removed-broadcast: "&8» &cTu clan ha roto la alianza con &b%clan%&c."
    clan-disbanded: "&8» &cTu clan ha roto la alianza con &b%clan% &cdebido a que fue eliminado."

    no-allies: "&8» &cTu clan no tiene alianzas."
    header:
      - " "
      - "&8&l» &7Alianzas de tu Clan"
      - ""
    entry: "&8● &7%clan% &8(&7%online%&8/&7%total%&8)"

    cannot-damage: "&8» &cNo puedes atacar a miembros de &b%clan% &cporque son aliados."

  rally:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    info-to-members: "&3[REUNIÓN] &fEl jugador &a%player% &fsolicita apoyo en &a%worldguard_region_name%&f."
    expired-info-to-members: "&4⚠ &cLa reunión ha expirado."
    expired-info-to-ally: "&4⚠ &cLa reunión del clan %clan% ha expirado."
    info-to-ally: "&3[REUNIÓN] &fEl jugador &a%player% &fdel clan &b%clan% &fsolicita apoyo en &a%worldguard_region_name%&f."

  base:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    info-to-members: "&3[BASE] &fEl jugador &a%player% &fha cambiado la base a &e%x%, %y%, %z%."
    need-higher-role: "&8» &cDebes ser al menos &eLÍDER &cpara cambiar la base."
    in-blacklisted-world: "&8» &cEstás en un mundo de la lista negra, no puedes irte/cambiar la base."
    no-exists: "&8» &cTu clan no tiene una base establecida."
    teleport: "&8» &aHas sido teletransportado a la base del clan."
    format: "&8» &cPara establecer la base de tu clan, usa: /clan base set."

  rename:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    already-exists: "&8» &cYa existe un clan con este nombre"
    info-to-members: "&3[RENOMBRAR] &fEl jugador &a%player% &fha cambiado el nombre del clan a %clan% con el tag %tag%&f."
    need-higher-role: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara cambiar el nombre."
    format: "&8» &cPara renombrar tu clan, usa: /clan rename (nombre) (tag)."

    already_exist: "&8» &cEl clan &b%clan% &cya existe."
    already_in_clan: "&8» &cYa estás en un clan. Usa &b/clan leave &cpara salir antes de renombrar."
    name_to_large: "&8» &cEl nombre del clan no puede exceder los &e16 &ccaracteres."
    renamed: "&8» &fHas renombrado el clan a &b%clan% &fcon el tag &b%tag%&f."
    invalid_name: "&8» &cEl nombre ingresado no es válido. Solo se permiten letras, números y algunos símbolos."
    cooldown: "&8» &cNecesitas esperar &e%time% &cpara volver a renombrar el clan."

    format:
      - "&8» &cUso: &f/clan info &b(nombre)"
      - "&7Muestra la información del clan, incluso si está desconectado."
    dont-exist: "&8» &cEl clan &b%name% &cno existe."
    header:
      - " "
      - "&7Clan &b%name% &8(&7%online%&f/&7%amount%&8) - &b%tag%"
      - "&8Miembro | Ultima conexión | Rol | Tiempo en el clan"

    online-player: "&8● &a%name% &8(&aConectado&8) - &b%role% - &8(%time_since_join%)"
    offline-player: "&8● &7%name% &8(&7%last_active%&8) - &b%role%  - &8(%time_since_join%)"

    footer:
      - " "
      - "&8Estadísticas:"
      - "&8» &fPuntos: &b%points% &8| &fAsesinatos: &b%kills% &8| &fMuertes: &b%deaths%"
      - "&8» &fDinero: &b%money%"
      - "&8» &fPuntuación Total: &e%score%"
      - "&8» &fAliados: &b%allies%"
      - "&8» &fEnemigos: &b%enemies%"

  friendlyfire:
    on-info-to-members: "&8» &fEl jugador &b%player% &fha &aactivado &fel PVP entre miembros del clan."
    off-info-to-members: "&8» &fEl jugador &b%player% &fha &cdesactivado &fel PVP entre miembros del clan."
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    need-higher-role: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara cambiar esta configuración."

  chat:
    format:
      - "&8» &cUso: &f/clan chat &b(enemy) (clan enemigo)"
      - "&8» &cUso: &f/clan chat &bally (clan aliado)"
      - "&7Usa solo &f/clan chat &7para alternar entre el chat global y el del clan."

    global: "&8» &fHas cambiado al chat &bGLOBAL&f."
    clan: "&8» &fHas cambiado al chat &bDEL CLAN&f."

    enemy: "&8» &fAhora puedes hablar con el clan enemigo &b%enemy_tag% &8(&7%enemy%&8)&f."
    enemy-format: "&8» &cUso: &f/clan chat enemy &b(clan enemigo)"
    enemy-offline: "&8» &cEl clan enemigo %enemy% no está conectado."
    no-found-enemy:
      - "&8» &cEl clan enemigo &b%enemy%&c no se encontró."
      - "&7Enemigos actuales: &b%enemies%"

    no-in-clan: "&8» &cNo perteneces a ningún clan."

    ally: "&8» &fAhora puedes hablar con el clan aliado &b%ally_tag% &8(&7%ally%&8)&f."
    ally-format: "&8» &cUso: &f/clan chat ally &b(clan aliado)"
    ally-offline: "&8» &cEl clan aliado %ally% no está conectado."
    no-found-ally:
      - "&8» &cEl clan aliado &b%ally%&c no se encontró."
      - "&7Aliados actuales: &b%allies%"

  invite:
    format: "&8» &cUso: &f/clan invite &b(accept/deny/jugador)"
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está conectado."
    yourself: "&8» &cNo puedes auto-invitarte."
    NO_LEADER: "&8» &cSolo el líder puede enviar invitaciones."
    NO_IN_CLAN: "&8» &cNo perteneces a ningún clan."
    ALREADY_IN_CLAN: "&8» &cEl jugador &b%target% &cya está en tu clan."
    ALREADY_IN_OTHER_CLAN: "&8» &cEl jugador &b%target% &cya pertenece al clan &b%tag% &8(&7%clan%&8)&c."
    ALREADY_INVITED: "&8» &cYa has invitado a este jugador."
    ALREADY_INVITED_BY_OTHER_CLAN: "&8» &cEl jugador ya ha sido invitado al clan &b%clan%&c."
    NO_INVITED: "&8» &cNo tienes invitaciones pendientes."
    MAX_MEMBERS: "&8» &cTu clan ha alcanzado el límite de &e%max% &cmiembros."
    DENIED: "&8» &fHas &crechazado &fla invitación al clan &b%tag% &8(&7%clan%&8)&f."
    INVITED: "&8» &fHas sido invitado al clan &b%tag% &8(&7%clan%&8)&f por &b%sender%&f."
    ACCEPTED: "&8» &fHas &aaceptado &fla invitación al clan &b%tag% &8(&7%clan%&8)&f."
    SEND: "&8» &fHas enviado una invitación a &b%target%&f."
    info-to-members:
      QUIT: "&8» &eEl jugador &b%target% &eha salido; la invitación ha expirado."
      DENIED: "&8» &eEl jugador &b%target% &chas rechazado &eunirse al clan."
      INVITED: "&8» &fEl líder &b%sender% &fha invitado a &b%target%&f."
      ACCEPTED: "&8» &fEl jugador &b%target% &fha &aaceptado &funirse al clan."

  kick:
    format:
      - "&8» &cUso: &f/clan kick &b(jugador) (razón)"
      - "&7Ejemplo: /clan kick &bPepito &fComportamiento inapropiado"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en tu clan."
    yourself: "&8» &cNo puedes expulsarte a ti mismo. Usa &b/clan leave&c."
    high-rank: "&8» &cNo puedes expulsar a alguien con un rango igual o superior al tuyo."
    min-rank: "&8» &cDebes ser al menos &eMOD &cpara expulsar jugadores."
    info-to-members: "&8» &fEl jugador &b%player% &fha expulsado a &b%target% &fpor: &e%reason%"
    info-to-kicked: "&8» &cHas sido expulsado del clan por &b%player% &c(razón: &e%reason%&c)."

  set-role:
    format:
      - "&8» &cUso: &f/clan setrole &b(jugador) (user/mod/coleader/leader)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en tu clan."
    yourself: "&8» &cNo puedes cambiar tu propio rol."
    high-rank: "&8» &cNo puedes modificar el rol de un jugador con rango igual o superior."
    need-high-rank: "&8» &cNo tienes el rango requerido para realizar esta acción."
    min-rank: "&8» &cSolo los &eSUB-LÍDERES &cpueden cambiar roles."
    info-to-members: "&8» &fEl jugador &b%player% &fha cambiado el rol de &b%target% &fa &b%target_role%&f."
    change-leader: "&8» &fEl liderazgo fue transferido de &b%player% &fa &b%target%&f."
    unexist-role: "&8» &cEl rol &b%role% &cno existe. Usa: &fuser, mod, coleader, leader."
    same-role: "&8» &cEl jugador ya tiene ese rol."
    leader-confirm:
      - "&e&lADVERTENCIA: &cusa /clan setrole &6%target% leader &c&lCONFIRM"
      - "&ePara dar el liderazgo a otra persona, automáticamente después"
      - "&ete convertirás en sub-líder."

  upgrade:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    max-level: "&8» &cLa mejora &b%upgrade% &cya ha alcanzado su nivel máximo."
    no-enough-balance: "&8» &cTu clan no tiene fondos suficientes. Requiere &e%amount%&c, disponible: &e%clan_balance%&c."
    info-upgrade: "&8» &fEl jugador &b%player% &fmejoró &b%upgrade% &fal nivel &b%level%&f."

  bank:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    format:
      - "&8» &cUso: &f/clan bank &b(deposit/withdraw) (cantidad)"
      - "&7Ejemplo: /clan bank deposit &b1000"
      - "&7Usa solo &f/clan bank &7para ver el saldo actual."
    error:
      POSITIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado grande."
      NEGATIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado pequeño."
      FOUND_SIGN_CHARACTER: "&8» &cNo incluyas signos + o - en la cantidad."
      FOUND_INVALID_NUMBER: "&8» &cLa cantidad &e%amount% &cno es válida."
      EMPTY_STRING: "&8» &cLa cantidad debe ser mayor a 0."
      cant-withdraw: "&8» &cError en la transacción. No se pudo retirar el dinero."
      no-has-enough-money: "&8» &cNo tienes &e%amount% &cpara depositar."
      clan-no-has-enough-money: "&8» &cEl clan no tiene fondos suficientes (&b%clan_amount%&c)."
    info: "&8» &fSaldo del clan: &b%amount%"
    successfully:
      deposit: "&8» &fEl jugador &b%player% &fdepositó &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."
      withdraw: "&8» &fEl jugador &b%player% &fretiró &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."

  enemy:
    format:
      - "&8» &cUso: &f/clan enemy &b(add/remove) (nombre)"
      - "&7Ejemplo: /clan enemy add &bClanDePepe"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    need-high-rank: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara modificar enemigos."
    max-enemies: "&8» &cTu clan ha alcanzado el límite de &e%max% &cenemigos."
    no-online: "&8» &cSolo puedes declarar enemigo a un clan que esté conectado."
    add: "&8» &fEl jugador &b%player% &fha declarado al clan &b%enemy_tag% &8(&7%enemy_name%&8)&f como enemigo."
    remove: "&8» &fEl jugador &b%player% &fha eliminado al clan &b%enemy% &fde la lista de enemigos."
    cant-remove: "&8» &cEl clan &b%enemy% &cno está en tu lista de enemigos."
    same-clan: "&8» &cNo puedes añadir a tu propio clan como enemigo."

  ally:
    format: "&8» &cUso: &f/clan ally &b<add|remove|accept|deny|cancel|list> (clan)"
    add-format: "&8» &cUso: &f/clan ally add &b(clan)"
    accept-format: "&8» &cUso: &f/clan ally accept &b(clan)"
    deny-format: "&8» &cUso: &f/clan ally deny &b(clan)"
    cancel-format: "&8» &cUso: &f/clan ally cancel &b(clan)"
    remove-format: "&8» &cUso: &f/clan ally remove &b(clan)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    min-rank: "&8» &cNecesitas ser al menos Sub-Líder para gestionar alianzas."
    clan-not-found: "&8» &cEl clan &b%clan% &cno fue encontrado."
    cannot-ally-yourself: "&8» &cNo puedes formar una alianza con tu propio clan."
    already-allied: "&8» &cYa estás aliado con &b%clan%&c."
    cannot-ally-enemy: "&8» &cNo puedes tener una alianza con &b%clan% &cporque son tus enemigos."
    max-allies: "&8» &cNo puedes tener más de &b%max% &calianzas."
    target-max-allies: "&8» &cEl clan &b%clan% &cya tiene el número máximo de alianzas."
    not-allied: "&8» &cNo estás aliado con &b%clan%&c."
    no-pending-request: "&8» &cNo hay ninguna solicitud de alianza pendiente con &b%clan%&c."
    no-permission: "&8» &cNo tienes permiso para gestionar alianzas."

    request-sent: "&8» &aSolicitud de alianza enviada a &b%clan%&a."
    request-received: "&8» &b%clan% &asolicita una alianza contigo &8(&7enviada por &b%sender%&8)"
    already-pending-request: "&8» &cYa hay una solicitud de alianza pendiente con %clan%"
    accepted: "&8» &aHas aceptado la alianza con &b%clan%&a."
    denied: "&8» &cHas rechazado la alianza con &b%clan%&c."
    cancelled: "&8» &cHas cancelado la solicitud de alianza con &b%clan%&c."
    removed: "&8» &aHas roto la alianza con &b%clan%&a."

    request-denied: "&8» &cEl clan &b%clan% &cha rechazado tu solicitud de alianza."
    request-cancelled: "&8» &cEl clan &b%clan% &cha cancelado su solicitud de alianza."
    added-broadcast: "&8» &a¡Tu clan se ha aliado con &b%clan%&a!"
    removed-broadcast: "&8» &cTu clan ha roto la alianza con &b%clan%&c."
    clan-disbanded: "&8» &cTu clan ha roto la alianza con &b%clan% &cdebido a que fue eliminado."

    no-allies: "&8» &cTu clan no tiene alianzas."
    header:
      - " "
      - "&8&l» &7Alianzas de tu Clan"
      - ""
    entry: "&8● &7%clan% &8(&7%online%&8/&7%total%&8)"

    cannot-damage: "&8» &cNo puedes atacar a miembros de &b%clan% &cporque son aliados."

  rally:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    info-to-members: "&3[REUNIÓN] &fEl jugador &a%player% &fsolicita apoyo en &a%worldguard_region_name%&f."
    expired-info-to-members: "&4⚠ &cLa reunión ha expirado."
    expired-info-to-ally: "&4⚠ &cLa reunión del clan %clan% ha expirado."
    info-to-ally: "&3[REUNIÓN] &fEl jugador &a%player% &fdel clan &b%clan% &fsolicita apoyo en &a%worldguard_region_name%&f."

  base:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    info-to-members: "&3[BASE] &fEl jugador &a%player% &fha cambiado la base a &e%x%, %y%, %z%."
    need-higher-role: "&8» &cDebes ser al menos &eLÍDER &cpara cambiar la base."
    in-blacklisted-world: "&8» &cEstás en un mundo de la lista negra, no puedes irte/cambiar la base."
    no-exists: "&8» &cTu clan no tiene una base establecida."
    teleport: "&8» &aHas sido teletransportado a la base del clan."
    format: "&8» &cPara establecer la base de tu clan, usa: /clan base set."

  rename:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    already-exists: "&8» &cYa existe un clan con este nombre"
    info-to-members: "&3[RENOMBRAR] &fEl jugador &a%player% &fha cambiado el nombre del clan a %clan% con el tag %tag%&f."
    need-higher-role: "&8» &cDebes ser al menos &eSUB-LÍDER &cpara cambiar el nombre."
    format: "&8» &cPara renombrar tu clan, usa: /clan rename (nombre) (tag)."

    already_exist: "&8» &cEl clan &b%clan% &cya existe."
    already_in_clan: "&8» &cYa estás en un clan. Usa &b/clan leave &cpara salir antes de renombrar."
    name_to_large: "&8» &cEl nombre del clan no puede exceder los &e16 &ccaracteres."
    renamed: "&8» &fHas renombrado el clan a &b%clan% &fcon el tag &b%tag%&f."
    invalid_name: "&8» &cEl nombre ingresado no es válido. Solo se permiten letras, números y algunos símbolos."
    cooldown: "&8» &cNecesitas esperar &e%time% &cpara volver a renombrar el clan."

```
{% endcode %}
