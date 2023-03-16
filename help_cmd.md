# /help で表示されるコマンド構文一覧

## Rel 1.19.70 オペレーター チートオン
```
/? <page: int>
/? [command: CommandName]
/alwaysday [lock: Boolean]
/camerashake add <player: target> [intensity: float] [seconds: float] [shakeType: CameraShakeType]
/camerashake stop [player: target]
/clear [player: target] [itemName: Item] [data: int] [maxCount: int]
/clearspawnpoint [player: target]
/clone <begin: x y z> <end: x y z> <destination: x y z> [maskMode: MaskMode] [cloneMode: CloneMode]
/clone <begin: x y z> <end: x y z> <destination: x y z> filtered <cloneMode: CloneMode> <tileName: Block> <blockStates: block states>
/connect <serverUri: text>
/damage <target: target> <amount: int> <cause: DamageCause> entity <damager: target>
/damage <target: target> <amount: int> [cause: DamageCause]
/daylock [lock: Boolean]
/deop <player: target>
/dialogue change <npc: target> <sceneName: string> [players: target]
/dialogue open <npc: target> <players: target> [sceneName: string]
/difficulty <difficulty: Difficulty>
/difficulty <difficulty: int>
/effect <player: target> <effect: Effect> [seconds: int] [amplifier: int] [hideParticles: Boolean]
/effect <player: target> clear
/enchant <player: target> <enchantmentId: int> [level: int]
/enchant <player: target> <enchantmentName: Enchant> [level: int]
/event entity <target: target> <eventName: string>
/execute <subcommand: Option_If_Unless> block <position: x y z> <block: Block> <blockStates: block states> [chainedCommand: ExecuteChainedOption_0]
/execute <subcommand: Option_If_Unless> block <position: x y z> <block: Block> [chainedCommand: ExecuteChainedOption_0]
/execute <subcommand: Option_If_Unless> blocks <begin: x y z> <end: x y z> <destination: x y z> <scan mode: BlocksScanMode> [chainedCommand: ExecuteChainedOption_0]
/execute <subcommand: Option_If_Unless> entity <target: target> [chainedCommand: ExecuteChainedOption_0]
/execute <subcommand: Option_If_Unless> score <target: target> <objective: string> <operation: compare operator> <source: target> <objective: string> [chainedCommand: ExecuteChainedOption_0]
/execute <subcommand: Option_If_Unless> score <target: target> <objective: string> matches <range: integer range> [chainedCommand: ExecuteChainedOption_0]
/execute align <axes: string> <chainedCommand: ExecuteChainedOption_0>
/execute anchored <eyes|feet> <chainedCommand: ExecuteChainedOption_0>
/execute as <origin: target> <chainedCommand: ExecuteChainedOption_0>
/execute at <origin: target> <chainedCommand: ExecuteChainedOption_0>
/execute facing <position: x y z> <chainedCommand: ExecuteChainedOption_0>
/execute facing entity <origin: target> <eyes|feet> <chainedCommand: ExecuteChainedOption_0>
/execute in <dimension: Dimension> <chainedCommand: ExecuteChainedOption_0>
/execute positioned <position: x y z> <chainedCommand: ExecuteChainedOption_0>
/execute positioned as <origin: target> <chainedCommand: ExecuteChainedOption_0>
/execute rotated <yaw: value> <pitch: value> <chainedCommand: ExecuteChainedOption_0>
/execute rotated as <origin: target> <chainedCommand: ExecuteChainedOption_0>
/execute run <command: command>
/fill <from: x y z> <to: x y z> <tileName: Block> <blockStates: block states> replace [replaceTileName: Block] [replaceBlockStates: block state]
/fill <from: x y z> <to: x y z> <tileName: Block> [blockStates: block states] [oldBlockHandling: FillMode]
/fog <victim: target> <mode: delete> <userProvideId: string>
/fog <victim: target> push <fogId: string> <userProvideId: string>
/function <name: filepath>
/gamemode <gameMode: GameMode> [player: target]
/gamemode <gameMode: int> [player: target]
/gamerule
/gamerule <rule: BoolGameRule> [value: Boolean]
/gamerule <rule: IntGameRule> [value: int]
/gametest clearall
/gametest create <testName: string> [width: int] [height: int] [depth: int]
/gametest pos
/gametest run <testName: string> <stopOnFailure: Boolean> <repeatCount: int> [rotationSteps: int]
/gametest run <testName: string> [rotationSteps: int]
/gametest runset [tag: string] [rotationSteps: int]
/gametest runthese
/gametest runthis
/give <player: target> <itemName: Item> [amount: int] [data: int] [components: json]
/help <page:int>
/help [command: CommandName]
/kick <name: target> <reason: massage>
/kill [target: target]
/list
/locate biome <biome: Biome>
/locate structure <structure: Structure> [useNewChunksOnly: Boolean]
/loot give <players: target> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot give <players: target> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot insert <position: x y z> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot insert <position: x y z> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot replace block <position: x y z> slot.container <slotId: int> <count: int> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot replace block <position: x y z> slot.container <slotId: int> <count: int> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot replace block <position: x y z> slot.container <slotId: int> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot replace block <position: x y z> slot.container <slotId: int> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> <count: int> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> <count: int> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/loot spawn <position: x y z> kill <entity: target> [<tool>|mainhand|offhand: string]
/loot spawn <position: x y z> loot <loot_table: string> [<tool>|mainhand|offhand: string]
/me <message: message>
/mobevent <event: MobEvent> [value: Boolean]
/msg <target: target> <message: message>
/music play <trackName: string> [volume: float] [fadeSeconds: float] [repeatMode: MusicRepeatMode]
/music queue <trackName: string> [volume: float] [fadeSeconds: float] [repeatMode: MusicRepeatMode]
/music stop [fadeSeconds: float]
/music volume <volume: float>
/op <player: target>
/particle <effect: string> [position: x y z]
/playanimation <entity: target> <animation: string> [next_state: string] [blend_out_time: float] [stop_expression: string] [controller: string]
/playsound <sound: string> [player: target] [position: x y z] [volume: float] [pitch: float] [minimumVolume: float]
/reload
/replaceitem block <position:x y z> slot.container <slotId: int> <itemName: Item> [amount: int] [data: int] [components: json]
/replaceitem block <position:x y z> slot.container <slotId: int> <oldItemHandling: ReplaceMode> <itemName: Item> [amount: int] [data: int] [components: json]
/replaceitem entity <target: target> <slotType: EntityEquipmentSlot> <slotId: int> <itemName: Item> [amount: int] [data: int] [components: json]
/replaceitem entity <target: target> <slotType: EntityEquipmentSlot> <slotId: int> <oldItemHandling: ReplaceMode> <itemName: Item> [amount: int] [data: int] [components: json]
/ride <riders: target> start_riding <ride: target> [teleportRules: TeleportRules] [howToFill: FillType]
/ride <riders: target> stop_riding
/ride <riders: target> summon_ride <entityType: EntityType> [rideRules: RideRules] [spawnEvent: string] [nameTag: string]
/ride <rides: target> evict_riders
/ride <rides: target> summon_rider <entity: EntityType> [spawnEvent: string] [nameTag: string]
/say <message: message>
/schedule on_area_loaded add <from: x y z> <to: x y z> <function: filepath>
/schedule on_area_loaded add circle <center: x y z> <radius: int> <function: filepath>
/schedule on_area_loaded add tickingarea <name: string> <function: filepath>
/scoreboard objectives add <objective: string> dummy [displayName: string]
/scoreboard objectives list
/scoreboard objectives remove <objective: string>
/scoreboard objectives setdisplay <list|sidebar> [objective: string] [ascending|descending]
/scoreboard objectives setdisplay belowname [objective: string]
/scoreboard players <add|remove|set> <player: target> <objective: string> <count: int>
/scoreboard players list [playername: target]
/scoreboard players operation <targetName: target> <targetObjective: string> <operation: operator> <selector: target> <objective: string>
/scoreboard players random <player: target> <objective: string> <min: int> <max: int>
/scoreboard players reset <player: target> [objective: string]
/scoreboard players test <player: target> <objective: string> <min: wildcard int> [max: wildcard int]
/script debugger close
/script debugger connect [host: string] [port: int]
/script debugger listen <port: int>
/script profiler start
/script profiler stop
/script watchdog exportstats
/setblock <position:x y z> <tileName: Block> [blockStates: block states] [replace|destroy|keep]
/setmaxplayers <maxPlayers: int>
/setworldspawn [spawnPoint: x y z]
/spawnpoint [player: target] [spawnPos: x y z]
/spreadplayers <x:value> <z:value> <spreadDistance: float> <maxRange: float> <victim: target>
/stopsound <player: target> [sound: string]
/structure delete <name: string>
/structure load <name: string> <to: x y z> [rotation: Rotation] [mirror: Mirror] [animationMode: StructureAnimationMode] [animationSeconds: float] [includeEntities: Boolean] [includeBlocks: Boolean] [waterlogged: Boolean] [integrity: float] [seed: string]
/structure load <name: string> <to: x y z> [rotation: Rotation] [mirror: Mirror] [includeEntities: Boolean] [includeBlocks: Boolean] [waterlogged: Boolean] [integrity: float] [seed: string]
/structure save <name: string> <from: x y z> <to: x y z> [includeEntities: Boolean] [savemode: StructureSaveMode] [includeBlocks: Boolean]
/structure save <name: string> <from: x y z> <to: x y z> [savemode: StructureSaveMode]
/summon <entityType: EntityType> <nameTag: string> [spawnPos: x y z]
/summon <entityType: EntityType> [spawnPos: x y z] [yRot: float] [xRot: float] [spawnEvent: string] [nameTag: string]
/tag <entity: target> <add|remove> <name: string>
/tag <entity: target> list
/teleport <destination: target> [checkForBlocks: Boolean]
/teleport <destination: x y z> [checkForBlocks: Boolean]
/teleport <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean]
/teleport <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean]
/teleport <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean]
/teleport <victim: target> <destination: target> [checkForBlocks: Boolean]
/teleport <victim: target> <destination: x y z> [checkForBlocks: Boolean]
/teleport <victim: target> <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean]
/teleport <victim: target> <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean]
/teleport <victim: target> <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean]
/tell <target: target> <message: message>
/tellraw <target: target> <raw json message: json>
/testfor <victim: target>
/testforblock <position: x y z> <tileName: Block> [blockStates: block states]
/testforblocks <begin: x y z> <end: x y z> <destination: x y z> [masked|all]
/tickingarea add <from: x y z> <to: x y z> [name: string] [preload: Boolean]
/tickingarea add circle <center: x y z> <radius: int> [name: string] [preload: Boolean]
/tickingarea list [all-dimansions: AllDimensions]
/tickingarea preload <name: string> [preload: Boolean]
/tickingarea preload <position: x y z> [preload: Boolean]
/tickingarea remove <name: string>
/tickingarea remove <position: x y z>
/tickingarea remove_all
/time add <amount: int>
/time query <time: TimeQuery>
/time set <amount: int>
/time set <time: TimeSpec>
/title <player: target> <title|subtitle|actionbar> <titleText: message>
/title <player: target> clear
/title <player: target> reset
/title <player: target> times <fadeIn: int> <stay: int> <fadeOut: int>
/titleraw <player: target> <titleLocation: TitleRawSet> <raw json titleText: json>
/titleraw <player: target> clear
/titleraw <player: target> reset
/titleraw <player: target> times <fadeIn: int> <stay: int> <fadeOut: int>
/toggledownfall
/tp <destination: target> [checkForBlocks: Boolean]
/tp <destination: x y z> [checkForBlocks: Boolean]
/tp <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean]
/tp <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean]
/tp <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean]
/tp <victim: target> <destination: target> [checkForBlocks: Boolean]
/tp <victim: target> <destination: x y z> [checkForBlocks: Boolean]
/tp <victim: target> <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean]
/tp <victim: target> <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean]
/tp <victim: target> <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean]
/w <target: target> <message: message>
/weather <clear|rain|thunder> [duration: int]
/weather query
/wsserver <serverUri: text>
/xp <amount: int> [player: target]
/xp <amount: int>L [player: target]
```
## Upcoming Creator Features (今後のクリエイター機能) オン
```
/volumearea add <identifier: string> <from: x y z> <to: x y z> [name: string]
/volumearea list [all-dimensions: VolumeAreaAllDimensions]
/volumearea remove <name: string>
/volumearea remove <position: x y z>
/volumearea remove_all
```
## Education Edition オン
```
/ability <player: target> <ability: Ability> <value: Boolean>
/ability <player: target> [ability: Ability]
/immutableworld [value: Boolean]
/wb
/worldbuilder
```
## BDS内
```
/allowlist <action: AllowListAction> [name: string]
/changesetting allow-cheats <value: Boolean>
/changesetting difficulty <value: Difficulty>
/changesetting difficulty <value: int>
/ops <action: PermissionsAction>
/parmission <action: PermissionsAction>
/save <mode: SaveMode>
/stop
/whitelist <action: AllowListAction> [name: string]
```
## Pre 1.19.80.21
```
/fill <from: x y z> <to: x y z> <tileName: Block> <blockStates: block states> replace <replaceTileName: Block> [replaceBlockStates: block state]
/fill <from: x y z> <to: x y z> <tileName: Block> [oldBlockHandling: FillMode]
/fill <from: x y z> <to: x y z> <tileName: Block> replace [replaceTileName: Block] [replaceBlockStates: block state]
/inputpermission query <targets: target> <permission: permission> [state: state]
/inputpermission set <targets: target> <permission: permission> <state: state>
/setblock <position:x y z> <tileName: Block> [replace|destroy|keep]
/summon <entityType: EntityType> [spawnPos: x y z] facing <lookAtEntity: target> [spawnEvent: string] [nameTag: string]
/summon <entityType: EntityType> [spawnPos: x y z] facing <lookAtPosition: x y z> [spawnEvent: string] [nameTag: string]
```
## 隠しコマンド
Fandom Wikiより
いくつかはBDSで実行可能
websocket とか Script API が関わる?
情報求
```
/agent ???
/closewebsocket ???
/dedicatedwsserver ???
/enableencryption ???
/getchunkdata <dimension: string> <chunkX: int> <chunkZ: int> <height: int>
/getchunks ???
/geteduserverinfo ???
/getlocalplayername ???
/getspawnpoint ???
/gettopsolidblock ???
/globalpause ???
/listd ???
/querytarget <target: target>
/replace ???
/takepicture <targetCamera: target> <targetPlayer: target>
/takepicture <cameraSpawnLocation: ???> <targetPlayer: target>
/takepicture <targetPlayer: target>
```