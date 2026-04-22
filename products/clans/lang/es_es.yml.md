---
icon: head-side-speak
---

# es\_ES.yml

```yaml
aliases:
  - "es_ES"
  - "es_AR"
  - "es_CL"
  - "es_MX"
  - "es_CO"
  - "es_PE"

messages:
  action-dont-registered: "&8» &cEsta acción no está registrada. Contacta a un administrador."
  in-process: "&8» &cEspera a que termine la tarea: %action% para el clan %clan%"
  roles:
    ADMINISTRATOR: "&4&lADMIN"
    LEADER: "&b&lLÍDER"
    CO_LEADER: "&3&lSUB-LÍDER"
    MOD: "&9&lMOD"
    USER: "&5&lUSUARIO"

  role-error-message:
    ADD_ALLY: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara crear una alianza."
    REMOVE_ALLY: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara eliminar una alianza."
    HANDLE_ALLY: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara aceptar/rechazar/cancelar una alianza."
    ADD_ENEMY: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara añadir un clan enemigo."
    REMOVE_ENEMY: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara eliminar un clan enemigo."
    DEPOSIT_BANK: "&8» &cNecesitas ser al menos &eUSUARIO &cpara depositar dinero en el banco del clan."
    WITHDRAW_BANK: "&8» &cNecesitas ser al menos &eLÍDER &cpara retirar dinero del banco del clan."
    KICK_PLAYER: "&8» &cNecesitas ser al menos &eMOD &cpara expulsar jugadores del clan."
    INVITE_PLAYER: "&8» &cNecesitas ser al menos &eMOD &cpara invitar jugadores al clan."
    DISBAND: "&8» &cNecesitas ser al menos &eLÍDER &cpara disolver el clan."
    RENAME: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara renombrar el clan."
    SET_BASE: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara establecer la base del clan."
    CLAN_CHAT: "&8» &cNecesitas ser al menos &eUSUARIO &cpara usar el chat del clan."
    ALLY_CHAT: "&8» &cNecesitas ser al menos &eUSUARIO &cpara usar el chat de alianza."
    ENEMY_CHAT: "&8» &cNecesitas ser al menos &eUSUARIO &cpara usar el chat enemigo."
    MODIFY_FRIENDLY_FIRE: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara modificar el fuego amigo."
    CHANGE_TAG: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara cambiar la etiqueta del clan."
    RALLY: "&8» &cNecesitas ser al menos &eUSUARIO &cpara convocar una reunión."
    UPGRADE: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara mejorar el clan."
    SET_ROLE: "&8» &cNecesitas ser al menos &eSUB-LÍDER &cpara cambiar el rol a otro jugador."

  permission-errors:
    USER_UPGRADE: "&8» &cNo tienes permiso para mejorar tu clan."
    USER_TAG: "&8» &cNo tienes permiso para cambiar la etiqueta de tu clan."
    USER_SETROLE: "&8» &cNo tienes permiso para cambiar los roles de los miembros."
    USER_RENAME: "&8» &cNo tienes permiso para renombrar tu clan."
    USER_RALLY: "&8» &cNo tienes permiso para convocar una reunión."
    USER_LIST: "&8» &cNo tienes permiso para ver la lista de clanes."
    USER_LEAVE: "&8» &cNo tienes permiso para abandonar tu clan."
    USER_KICK: "&8» &cNo tienes permiso para expulsar miembros de tu clan."
    USER_INVITE: "&8» &cNo tienes permiso para gestionar invitaciones al clan."
    USER_INFO: "&8» &cNo tienes permiso para ver información del clan."
    USER_FRIENDLYFIRE: "&8» &cNo tienes permiso para gestionar la configuración de fuego amigo."
    USER_ENEMY: "&8» &cNo tienes permiso para gestionar enemigos."
    USER_DISBAND: "&8» &cNo tienes permiso para disolver tu clan."
    USER_CREATE: "&8» &cNo tienes permiso para crear un clan."
    USER_CHAT: "&8» &cNo tienes permiso para usar las funciones del chat del clan."
    USER_BASE: "&8» &cNo tienes permiso para gestionar la base de tu clan."
    USER_BANK: "&8» &cNo tienes permiso para gestionar el banco del clan."
    USER_ALLY: "&8» &cNo tienes permiso para gestionar alianzas."
    USER_USE: "&8» &cNo tienes permiso para usar comandos del clan."

  format:
    - "&3&lRunithClans" # Puedes usar colores hexadecimales, ejemplo: #AFCF21
    - " "
    - "&fComandos Disponibles &7→"
    - " &8● &bcreate &9(nombre) (etiqueta) &8- &fCrear un clan"
    - " &8● &bdisband &8- &fEliminar tu clan"
    - " &8● &bleave &8- &fAbandonar tu clan"
    - " &8● &bkick &9(jugador) &8- &fExpulsar un jugador"
    - " &8● &btag &9(nueva) &8- &fCambiar la etiqueta del clan"
    - " &8● &blist &9(página) &8- &fMostrar clanes conectados"
    - " &8● &binfo &9(clan) &8- &fMostrar información del clan"
    - " &8● &bchat &9(enemigo) (clan enemigo) &8- &fCambiar entre chats"
    - " &8● &binvite &9(aceptar/rechazar/jugador) &8- &fGestionar invitaciones"
    - " &8● &bsetrole &9(jugador) (rol) &8- &fCambiar el rol de un miembro"
    - " &8● &bbank &9(retirar/depositar) (cantidad) &8- &fGestionar el banco del clan"
    - " &8● &bally &9(añadir/eliminar/listar) (nombre) &8- &fGestionar alianzas"
    - " &8● &benemy &9(añadir/eliminar) (nombre) &8- &fGestionar enemigos"
    - " &8● &bupgrades &8- &fComprar mejoras del clan"
    - " &8● &bbase &9(establecer) &8- &fIr a/cambiar la base del clan"
    - " &8● &brally &8- &fConvocar a todos tus miembros"
    - " &8● &bfriendlyfire &8- &fActivar o desactivar PVP entre miembros"
    - " &8● &brename &9(nombre) (etiqueta) &8- &fRenombrar el clan"

  create:
    format:
      - "&8» &cUso: &f/clan create &b(nombre) (etiqueta)"
      - "&7Ejemplo: /clan create &bLosValientes &7(LV)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    already_exist: "&8» &cEl clan &b%clan% &cya existe."
    already_in_clan: "&8» &cYa estás en un clan. Usa &b/clan leave &cpara salir antes de crear otro."
    name_to_large: "&8» &cEl nombre del clan no puede exceder los &e16 &ccaracteres."
    created: "&8» &fHas creado el clan &b%clan% &fcon la etiqueta &b%tag%&f."
    invalid_name: "&8» &cEl nombre ingresado no es válido. Solo se permiten letras, números y algunos símbolos."

  disband:
    confirm:
      - "&8» &cUsa &f/clan disband &4&lconfirm &cpara confirmar."
      - "&e⚠ &6Esta acción es permanente y eliminará todas las estadísticas del clan."
      - "&7Si solo deseas transferir el liderazgo, usa &b/clan setrole (jugador) leader&7."
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    info-to-members: "&8» &6Tu clan ha sido disuelto por el líder &b%leader%&6."

  leave:
    is-leader: "&8» &cNo puedes abandonar el clan siendo el líder. Usa &b/clan disband &co transfiere el liderazgo."
    successfully: "&8» &fHas abandonado el clan."
    info-to-members: "&8» &eEl jugador &b%player% &eha abandonado el clan."
    no-in-clan: "&8» &cNo perteneces a ningún clan."

  tag:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    format:
      - "&8» &cUso: &f/clan tag &b(nueva_etiqueta)"
      - "&7Ejemplo: /clan tag &bLosDuros"
    info-to-members: "&8» &6El jugador &b%player% &6ha cambiado la etiqueta del clan a &b%name%&6."
    invalid:
      - " "
      - "&8» &cLa etiqueta solo puede contener &eletras&c, &enúmeros&c y símbolos válidos:"
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
      - "&7Muestra información del clan, incluso si está offline."
    dont-exist: "&8» &cEl clan &b%name% &cno existe."
    header:
      - " "
      - "&7Clan &b%name% &8(&7%online%&f/&7%amount%&8) - &b%tag%"
      - "&8Miembro | Última Actividad | Rol | Tiempo desde que se unió"

    online-player: "&8● &a%name% &8(&aEn línea&8) - &b%role% - &8(%time_since_join%)"
    offline-player: "&8● &7%name% &8(&7%last_active%&8) - &b%role%  - &8(%time_since_join%)"

    footer:
      - " "
      - "&8Estadísticas:"
      - "&8» &fPuntos: &b%points% &8| &fMuertes: &b%kills% &8| &fDefunciones: &b%deaths%"
      - "&8» &fDinero: &b%money%"
      - "&8» &fPuntuación Total: &e%score%"
      - "&8» &fAliados: &b%allies%"
      - "&8» &fEnemigos: &b%enemies%"

  friendlyfire:
    on-info-to-members: "&8» &fEl jugador &b%player% &fha &aactivado &f el PVP entre miembros del clan."
    off-info-to-members: "&8» &fEl jugador &b%player% &fha &cdesactivado &f el PVP entre miembros del clan."
    no-in-clan: "&8» &cNo perteneces a ningún clan."

  chat:
    format:
      - "&8» &cUso: &f/clan chat &b(enemigo) (clan enemigo)"
      - "&8» &cUso: &f/clan chat &baliado (clan aliado)"
      - "&7Usa solo &f/clan chat &7para cambiar entre el chat global y del clan."

    global: "&8» &fHas cambiado al chat &bGLOBAL&f."
    clan: "&8» &fHas cambiado al chat &bDEL CLAN&f."

    enemy: "&8» &fAhora puedes hablar con el clan enemigo &b%enemy_tag% &8(&7%enemy%&8)&f."
    enemy-format: "&8» &cUso: &f/clan chat enemy &b(clan enemigo)"
    enemy-offline: "&8» &cEl clan enemigo %enemy% no está conectado."
    no-found-enemy:
      - "&8» &cClan enemigo &b%enemy%&c no encontrado."
      - "&7Enemigos actuales: &b%enemies%"

    no-in-clan: "&8» &cNo perteneces a ningún clan."

    ally: "&8» &fAhora puedes hablar con el clan aliado &b%ally_tag% &8(&7%ally%&8)&f."
    ally-format: "&8» &cUso: &f/clan chat ally &b(clan aliado)"
    ally-offline: "&8» &cEl clan aliado %ally% no está conectado."
    no-found-ally:
      - "&8» &cClan aliado &b%ally%&c no encontrado."
      - "&7Aliados actuales: &b%allies%"

  invite:
    format: "&8» &cUso: &f/clan invite &b(aceptar/rechazar/jugador)"
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en línea."
    yourself: "&8» &cNo puedes invitarte a ti mismo."
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
      QUIT: "&8» &eEl jugador &b%target% &eha abandonado; la invitación ha expirado."
      DENIED: "&8» &eEl jugador &b%target% &eha &crechazado &eunirse al clan."
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
    info-to-members: "&8» &fEl jugador &b%player% &fha expulsado a &b%target% &fpor: &e%reason%"
    info-to-kicked: "&8» &cHas sido expulsado del clan por &b%player% &c(razón: &e%reason%&c)."

  set-role:
    format:
      - "&8» &cUso: &f/clan setrole &b(jugador) (usuario/mod/sublider/lider)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    target-dont-exist: "&8» &cEl jugador &b%target% &cno está en tu clan."
    yourself: "&8» &cNo puedes cambiar tu propio rol."
    high-rank: "&8» &cNo puedes modificar el rol de un jugador con un rango igual o superior."
    need-high-rank: "&8» &cNo tienes el rango requerido para realizar esta acción."
    info-to-members: "&8» &fEl jugador &b%player% &fha cambiado el rol de &b%target% &fa &b%target_role%&f."
    change-leader: "&8» &fEl liderazgo fue transferido de &b%player% &fa &b%target%&f."
    unexist-role: "&8» &cEl rol &b%role% &cno existe. Usa: &fusuario, mod, colider, líder."
    same-role: "&8» &cEl jugador ya tiene ese rol."
    leader-confirm:
      - "&e&lADVERTENCIA: &cusa /clan setrole &6%target% leader &c&lCONFIRMAR"
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
      - "&8» &cUso: &f/clan bank &b(depositar/retirar) (cantidad)"
      - "&7Ejemplo: /clan bank deposit &b1000"
      - "&7Usa solo &f/clan bank &7para ver el saldo actual."
    error:
      POSITIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado grande."
      NEGATIVE_OVERFLOW: "&8» &cEl número ingresado es demasiado bajo."
      FOUND_SIGN_CHARACTER: "&8» &cNo incluyas signos + o - en la cantidad."
      FOUND_INVALID_NUMBER: "&8» &cLa cantidad &e%amount% &cno es válida."
      EMPTY_STRING: "&8» &cLa cantidad debe ser mayor que 0."
      cant-withdraw: "&8» &cError de transacción. No se pudo retirar el dinero."
      no-has-enough-money: "&8» &cNo tienes &e%amount% &cpara depositar."
      clan-no-has-enough-money: "&8» &cEl clan no tiene fondos suficientes (&b%clan_amount%&c)."
    info: "&8» &fSaldo del clan: &b%amount%"
    successfully:
      deposit: "&8» &fEl jugador &b%player% &fdepositó &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."
      withdraw: "&8» &fEl jugador &b%player% &fretiró &b%amount% &f(&7%old_amount% ➜ %new_amount%&f)."

  enemy:
    format:
      - "&8» &cUso: &f/clan enemy &b(añadir/eliminar) (nombre)"
      - "&7Ejemplo: /clan enemy add &bClanDePepe"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    max-enemies: "&8» &cTu clan ha alcanzado el límite de &e%max% &cenemigos."
    no-online: "&8» &cSolo puedes declarar enemigo a un clan conectado."
    add: "&8» &fEl jugador &b%player% &fha declarado al clan &b%enemy_tag% &8(&7%enemy_name%&8)&f como enemigo."
    remove: "&8» &fEl jugador &b%player% &fha eliminado al clan &b%enemy% &fde la lista de enemigos."
    cant-remove: "&8» &cEl clan &b%enemy% &cno está en tu lista de enemigos."
    same-clan: "&8» &cNo puedes añadir tu propio clan como enemigo."

  ally:
    format: "&8» &cUso: &f/clan ally &b<añadir|eliminar|aceptar|rechazar|cancelar|listar> (clan)"
    add-format: "&8» &cUso: &f/clan ally add &b(clan)"
    accept-format: "&8» &cUso: &f/clan ally accept &b(clan)"
    deny-format: "&8» &cUso: &f/clan ally deny &b(clan)"
    cancel-format: "&8» &cUso: &f/clan ally cancel &b(clan)"
    remove-format: "&8» &cUso: &f/clan ally remove &b(clan)"
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    clan-not-found: "&8» &cEl clan &b%clan% &cno fue encontrado."
    cannot-ally-yourself: "&8» &cNo puedes formar una alianza con tu propio clan."
    already-allied: "&8» &cYa estás aliado con &b%clan%&c."
    cannot-ally-enemy: "&8» &cNo puedes tener una alianza con &b%clan% &cporque son tus enemigos."
    max-allies: "&8» &cNo puedes tener más de &b%max% &calianzas."
    target-max-allies: "&8» &cEl clan &b%clan% &cya tiene el número máximo de alianzas."
    not-allied: "&8» &cNo estás aliado con &b%clan%&c."
    no-pending-request: "&8» &cNo hay una solicitud de alianza pendiente con &b%clan%&c."
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
    clan-disbanded: "&8» &cTu clan ha roto la alianza con &b%clan% &cya que fue eliminado."

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
    in-blacklisted-world: "&8» &cEstás en un mundo en lista negra, no puedes ir/cambiar la base."
    no-exists: "&8» &cTu clan no tiene una base establecida."
    teleport: "&8» &aHas sido enviado a la base del clan."
    format: "&8» &cPara establecer la base de tu clan, usa: /clan base set."

  rename:
    no-in-clan: "&8» &cNo perteneces a ningún clan."
    already-exists: "&8» &cYa existe un clan con este nombre"
    info-to-members: "&3[CAMBIO DE NOMBRE] &fEl jugador &a%player% &fha cambiado el nombre del clan a %clan% con la etiqueta %tag%&f."
    format: "&8» &cPara renombrar tu clan, usa: /clan rename (nombre) (etiqueta)."

    already_exist: "&8» &cEl clan &b%clan% &cya existe."
    already_in_clan: "&8» &cYa estás en un clan. Usa &b/clan leave &cpara salir antes de crear otro."
    name_to_large: "&8» &cEl nombre del clan no puede exceder los &e16 &ccaracteres."
    renamed: "&8» &fHas renombrado el clan a &b%clan% &fcon la etiqueta &b%tag%&f."
    invalid_name: "&8» &cEl nombre ingresado no es válido. Solo se permiten letras, números y algunos símbolos."
    cooldown: "&8» &cNecesitas esperar &e%time% &cantes de volver a renombrar el clan"
```
