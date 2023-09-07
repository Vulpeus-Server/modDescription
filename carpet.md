# carpet

このドキュメント内では
`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

[carpet公式ドキュメント](https://github.com/gnembon/fabric-carpet/wiki/Current-Available-Settings)

## 目次
<details>
  <summary>general</summary>
  <li><a href="#carpet-1">carpet</a></li>
</details>

<details>
  <summary>rules</summary>
  <li><a href="#allowspawningofflineplayers">allowSpawningOfflinePlayers</a></li>
  <li><a href="#anticheatdisabled">antiCheatDisabled</a></li>
  <li><a href="#carpetcommandpermissionlevel">carpetCommandPermissionLevel</a></li>
  <li><a href="#carpets">carpets</a></li>
  <li><a href="#chainstone">chainStone</a></li>
  <li><a href="#cleanlog">cleanLog</a></li>
  <li><a href="#commanddistance">commandDistance</a></li>
  <li><a href="#commanddraw">commandDraw</a></li>
  <li><a href="#commandinfo">commandInfo</a></li>
  <li><a href="#commandlog">commandLog</a></li>
  <li><a href="#commandPerimeterinfo">commandPerimeterInfo</a></li>
  <li><a href="#commandplayer">commandPlayer</a></li>
  <li><a href="#commandprofile">commandProfile</a></li>
  <li><a href="#commandscript">commandScript</a></li>
  <li><a href="#commandscriptace">commandScriptACE</a></li>
  <li><a href="#commandspawn">commandSpawn</a></li>
  <li><a href="#commandtick">commandTick</a></li>
  <li><a href="#commandtrackingai">commandTrackingAI</a></li>
  <li><a href="#creativeflydrag">creativeFlyDrag</a></li>
  <li><a href="#creativeflyspeed">creativeFlySpeed</a></li>
  <li><a href="#creativenoclip">creativeNoClip</a></li>
  <li><a href="#creativeplayersloadchunks">creativePlayersLoadChunks</a></li>
  <li><a href="#ctrlqcraftingfix">ctrlQCraftingFix</a></li>
  <li><a href="#custommotd">customMOTD</a></li>
  <li><a href="#defaultloggers">defaultLoggers</a></li>
  <li><a href="#desertshrubs">desertShrubs</a></li>
  <li><a href="#explosionNoblockdamage">explosionNoBlockDamage</a></li>
  <li><a href="#fastredstonedust">fastRedstoneDust</a></li>
  <li><a href="#filllimit">fillLimit</a></li>
  <li><a href="#fillupdates">fillUpdates</a></li>
  <li><a href="#flippincactus">flippinCactus</a></li>
  <li><a href="#fogoff">fogOff</a></li>
  <li><a href="#forceloadlimit">forceloadLimit</a></li>
  <li><a href="#hardcodetntangle">hardcodeTNTangle</a></li>
  <li><a href="#hoppercounters">hopperCounters</a></li>
  <li><a href="#huskspawningintemples">huskSpawningInTemples</a></li>
  <li><a href="#interactionUpdates">interactionUpdates</a></li>
  <li><a href="#lagfreespawning">lagFreeSpawning</a></li>
  <li><a href="#lightningKkllsdropsfix">lightningKillsDropsFix</a></li>
  <li><a href="#liquiddamagedisabled<">liquidDamageDisabled</a></li>
  <li><a href="#maxentitycollisions">maxEntityCollisions</a></li>
  <li><a href="#mergetnt">mergeTNT</a></li>
  <li><a href="#missingtools">missingTools</a></li>
  <li><a href="#moreblueskulls">moreBlueSkulls</a></li>
  <li><a href="#movableamethyst">movableAmethyst</a></li>
  <li><a href="#movableblockentities">movableBlockEntities</a></li>
  <li><a href="#optimizedtnt">optimizedTNT</a></li>
  <li><a href="#perfpermissionlevel">perfPermissionLevel</a></li>
  <li><a href="#persistentparrots">persistentParrots</a></li>
  <li><a href="#piglinsspawninginbastions">piglinsSpawningInBastions</a></li>
  <li><a href="#pingplayerlistlimit">pingPlayerListLimit</a></li>
  <li><a href="#placementrotationfix">placementRotationFix</a></li>
  <li><a href="#portalcreativedelay">portalCreativeDelay</a></li>
  <li><a href="#portalsurvivaldelay">portalSurvivalDelay</a></li>
  <li><a href="#pushlimit">pushLimit</a></li>
  <li><a href="#quasiconnectivity">quasiConnectivity</a></li>
  <li><a href="#railpowerlimit">railPowerLimit</a></li>
  <li><a href="#renewableblackstone">renewableBlackstone</a></li>
  <li><a href="#renewablecoral">renewableCoral</a></li>
  <li><a href="#renewabledeepslate">renewableDeepslate</a></li>
  <li><a href="#renewablesponges">renewableSponges</a></li>
  <li><a href="#rotatorblock">rotatorBlock</a></li>
  <li><a href="#scriptsappstore">scriptsAppStore</a></li>
  <li><a href="#scriptsautoload">scriptsAutoload</a></li>
  <li><a href="#scriptsdebugging">scriptsDebugging</a></li>
  <li><a href="#scriptsoptimization">scriptsOptimization</a></li>
  <li><a href="#sculksensorrange">sculkSensorRange</a></li>
  <li><a href="#shulkerspawninginendcities">shulkerSpawningInEndCities</a></li>
  <li><a href="#silverfishdropgravel">silverFishDropGravel</a></li>
  <li><a href="#simulationdistance">simulationDistance</a></li>
  <li><a href="#smoothclientanimations">smoothClientAnimations</a></li>
  <li><a href="#spawnchunkssize">spawnChunksSize</a></li>
  <li><a href="#stackableshulkerboxes">stackableShulkerBoxes</a></li>
  <li><a href="#structureblockignored">structureBlockIgnored</a></li>
  <li><a href="#structureblocklimit">structureBlockLimit</a></li>
  <li><a href="#structureblockoutlinedistance">structureBlockOutlineDistance</a></li>
  <li><a href="#summonnaturallightning">summonNaturalLightning</a></li>
  <li><a href="#supersecretsetting">superSecretSetting</a></li>
  <li><a href="#thickfungusgrowth">thickFungusGrowth</a></li>
  <li><a href="#ticksyncedworldborders">tickSyncedWorldBorders</a></li>
  <li><a href="#tntdonotupdate">tntDoNotUpdate</a></li>
  <li><a href="#tntprimermomentumremoved">tntPrimerMomentumRemoved</a></li>
  <li><a href="#tntrandomrange">tntRandomRange</a></li>
  <li><a href="#updatesuppressionblock">updateSuppressionBlock</a></li>
  <li><a href="#viewdistance">viewDistance</a></li>
  <li><a href="#xpfromexplosions">xpFromExplosions</a></li>
  <li><a href="#xpnocooldown">xpNoCooldown</a></li>
</details>

<details>
  <summary>[counter](#counter)</summary>
  <li>realtime</li>
  <li>reset</li>
</details>

<details>
  <summary>[distance](#distance)</summary>
  <li>to</li>
  <li>from</li>
</details>


<!--
+ general
+ rule
+ counter
+ distance
+ draw
+ info
+ log
+ tick
+ perimeterinfo
+ profile
+ player
+ spawn
+ script
-->

## general
### carpet
  + `/carpet`<br>
    現在変更されているcarpetの設定、導入されているcarpetのバージョン、カテゴリーを表示する。
  + `/carpet list <category>`<br>
    利用できるcarpet ruleを**すべて**表示する。`<category>`を指定した場合、紐づけられたruleを表示する。
  + `/carpet list default`<br>
    `carpet.conf`に記録されているルールを表示する。
  + `/carpet setDefault [rule] [value]`<br>
    `[rule]`で指定したcarpet ruleのデフォルトの値を`[value]`で指定した値にする。

    >[!note]
    >`/carpet [rule] [value]`を使用し値が正常に変更された場合、通知とともにそえられる`change permanently?`を右クリックすることでその値がすでに入力されたコマンドが準備される。
  + `/carpet removeDefault <rule>`<br>
    `[rule]`で指定したcarpet ruleのデフォルトの値を`carpet.conf`から削除し、初期値にする。

<!--
### perimeter info
perimeterに関する情報を表示する。opレベル0を要求する。
#### `/perimeterinfo <coordinate>　<mob>`
`<coordinate>`を中心とした半径128の球体内に`<mob>`が湧くことができるブロックを表示する。
`<coordinate>`を指定しなかった場合現在の座標(`~ ~ ~`)が、`<mob>`を指定しなかった場合すべての存在するmobが指定される。
### info
指定した情報を表示する。opレベル0を要求する。WorldEditによって完全に代替される予定であるとのこと。
#### `/info block [coordinate] <grep>`
`[coordinate]`に関する情報を表示する。`<grep>`によって表示する情報を指定することが可能。
#### `/info entity [target] <grep>`
`[target]`に関する情報を表示する。`<grep>`によって表示する情報を指定することが可能。
-->

## rules
`/carpet [rule] <value>`によって変更することができる。
### ~~allowSpawningOfflinePlayers~~
  オフラインのプレイヤーを召喚できるかを設定できる。
  オフラインのプレイヤーは`/player [mcid] [spawn | shadow]`によるものではないことを確認。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### antiCheatDisabled
  バニラ標準のアンチチートを無効化する。アンチチートにはプレイヤーのリーチ制限や移動量制限などが含まれ、それぞれが数値上の最大値まで許容することができるようになる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### carpetCommandPermissionLevel
  `/carpet`コマンドを使用できるパーミッションレベルを指定する。`ops`では`/op`で付与された人のみであるが、`2` `4`はそれぞれの数値以上のパーミッションを保持しているプレイヤーにが使うことができる。

  >[!note]
  >現在たいち鯖では最大のパーミッションレベルが3になっている。
  + 初期値 : `ops`
  + 使用できる値 : `ops` `2` `4`
### carpets
  carpetを置くことで権限のない人でも特定のコマンドのみ使えるようにする。
  以下は使用できるコマンドのリストである。
  | color  | command                                      |
  |:------:|:---------------------------------------------|
  | gray   | `/info block ~ ~-1 ~`                        |
  | black  | `/spawn entities`                            |
  | brown  | `/distance from ~ ~ ~ ` `/distance to ~ ~ ~` |
  | pink   | `/spawn list ~ ~-1 ~`                        |
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + info
    + spawn
    + [distance](#distance)
### chainStone
チェーンを長いほうの端でスライムのように接続でき、かつほかのブロックとも接続できるようにする。`stick_to_all`を指定するとすべての方向について接続する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `stick_to_all`
### ~~cleanLog~~
 どのログがどのように消されるかは謎。

 **クライアントのみ**
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### commandDistance
  `/distance`を使用できるプレイヤーを指定する。`true` `false`ではopの所持の如何を問わず指定することができる。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [distance](#distance)
### commandDraw
  `/draw`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + draw
### commandInfo
  `/info`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + info
### commandLog
  `/log`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + log
### commandPerimeterInfo
  `/perimeterinfo`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + perimeterInfo
### commandPlayer
  `/player`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + player
### commandProfile
  `/profile`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + profile
### commandScript
  `/script`のscript作成を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + script
### commandScriptACE
  `/script load` `/script run`を使用できるプレイヤーを指定する。appが実行するときのopレベルでもある。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + script
### commandSpawn
  `/spawn`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + spawn
### commandTick
  `/tick`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + tick
### commandTrackingAI
  `/track`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + track
### creativeFlyDrag
  クリエイティブにおける空気抵抗(慣性の減衰度合い)を設定する。0で一切減衰せず、1でBEのようにストッピングができるようになる。

  **クライアントのみ**
  + 初期値 : `0.09`
  + 使用できる値 : `double`
### creativeFlySpeed
  クリエイティブにおける浮遊時の飛行速度を設定する。
  
  **クライアントのみ**
  + 初期値 : `1.0`
  + 使用できる値 : `double`
### creativeNoClip
  クリエイティブにおける飛行状態でブロックを貫通できるようにする。
  クライアントと鯖の双方に設定があるため、同じ設定にしないと動作が不安定になる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### creativePlayersLoadChunks
  クリエイティブのプレイヤーが周囲のチャンクをロードするかを設定する。
  >[!note]
  >スペクテイターモードについては`/gamerule spectatorsGenerateChunks`によって設定可能。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### ctrlQCraftingFix
  ctrlQによる一括排出をクラフトの結果欄でも機能するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### ~customMOTD~
  MOTD is なに
  + 初期値 : `_`
  + 使用できる値 : `string`
### defaultLoggers
  鯖に入ったときに表示するログの初期値。ただしsetDefaultを設定しないと再起動によって初期値に戻る。
  `tps,mobcaps,counter`のように、カンマで常げることでサジェストされたもの以外も指定できる。
  + 初期値 : `none`
  + 使用できる値 : `string`
  + 関連項目
    + log
### desertShrubs
  苗木が砂漠を含めた暑い気候および水のアクセスができない場所で枯れ木にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### explosionNoBlockDamage
  爆発ダメージを起こさなくする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### fastRedstoneDust
  redstone dustのupdate orderを複数回更新される場所を一回のみにすることで最適化がされる。 
  >[!note]
  >壊れる回路があるので注意。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`  
### fillLimit
  fillやcloneのブロック数制限を変更する。ただしゲームルールに同様の機能があり、そちらの数値に上書きされる。
  + 初期値 : `32768`
  + 使用できる値 : `integer`
### fillUpdates
  fillやclone、setblockによるblock updateを発生させないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [interactionUpdates](#interactionupdates)
### flippinCactus
  サボテンをメインハンドに持っている時、ホッパーやオブザーバーなど、方向をもつブロックの一部を右クリックするとその方向をupdateなしで回転もしくは反転できるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [rotatorCactus](#rotatorblock)
### fogOff
  ネザーにおよびエンドにおけるfog(霧)を消すようにする。

  **クライアントのみ**
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### forceloadLimit
  `/forceload`の上限を変更する。
  + 初期値 : `256`
  + 使用できる値 : `integer`
### hardcodeTNTangle
  tntの着火時に起きる水平方向の移動の計算方式を変更する。デフォルトは-1.0であり、これは変更しない(=ランダムである)ことを意味する。0から2πの範囲でその回転を指定できる。
  + 初期値 : `-1.0`
  + 使用できる値 : `double`
### hopperCounters
  `/counter`を有効にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [counter](#counters)
### huskSpawningInTemples
  ピラミッドではハスクのみがスポーンできるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### interactionUpdates
  ブロックを置くときにblock updateを発生させないようにする。
  + 初期値 : `true`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [fillUpdates](#fillupdates)
### lagFreeSpawning
  mobのスポーンを最適化する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### language
  carpetで使用する言語を変更する。
  + 初期値 : `en_us`
  + 使用できる値 : `en_us` `fr_fr` `pt_br` `zh_cn` `zh_tw`
### lightningKillsDropsFix
  [MC-206922](https://bugs.mojang.com/browse/MC-206922)を修正する。
  落雷がmobをキルした場合もmobがドロップすべきアイテムをドロップするようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### liquidDamageDisabled
  流体によるブロックの破壊を起こさなくする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### maxEntityCollisions
  一つのentityが持つ最大の当たり判定の数。0で無制限。非不整数でなければいけない。
  + 初期値 : `0`
  + 使用できる値 : `interger`
### mergeTNT
  着火されたtntが同一のfuseを持つ場合それらを起爆したときに同様の爆発ダメージ及びモーメントを与える一つのentityとする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### missingTools
  ガラスの適正ツールがつるはしとなる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### moreBlueSkulls
  witherによって出される青いskullの確率を上げる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### movableAmethyst
  芽の生えたアメジストをピストンによって移動できるようにする。また、シルクタッチのついた適正ツールで掘られた場合にはアイテムとしてドロップするようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### movableBlockEntities
  block entityをピストンにより移動可能にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`  
### optimizedTNT
  tntが同じ座標や流体内で爆発したときの最適化をする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### ~~perfPermissionLevel~~
  `/perf`が使用できる権限を変更する。**しかし`/perf`が確認できなかった。**
  + 初期値 : `4`
  + 使用できる値 : `2` `4`
### persistentParrots
  オウムがダメージをうけるまで常に肩に乗るようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### piglinsSpawningInBastions
  ピグリン、ピグリンブルート、ホグリンがbastionで自然スポーンすることができるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### pingPlayerListLimit
  ping playerのサンプル数の上限を設定する。非負整数である必要がある。
  + 初期値 : `12`
  + 使用できる値 : `integer`  
### placementRotationFix
  プレイヤーが高速で視点を動かしたときに設置されたブロックが回転するバグを修正する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### portalCreativeDelay
  プレイヤーがクリエイティブでネザーポータルを通過するために必要な時間を設定する。単位はgtで0から72000までをとる。
  + 初期値 : `0`
  + 使用できる値 : `integer`
  + 関連項目
    + [portalSurvivalDelay](#portalsurvivaldelay)
### portalSurvivalDelay
  プレイヤーがサバイバルでネザーポータルを通過するために必要な時間を設定する。単位はgtで0から72000までの整数値をとる。
  + 初期値 : `80`
  + 使用できる値 : `integer`
  + 関連項目
    + [creativePortalDelay](#portalcreativedelay)
### pushLimit
  ピストンが押せるブロックの最大量を決める必要がある。1から1024までの整数値をとる。
  + 初期値 : `12`
  + 使用できる値 : `integer`
### quasiConnectivity
  ピストンとドロッパー、ディスペンサーの準接続をおこさないようにする。
  + 初期値 : `true`
  + 使用できる値 : `true` `false`
### railPowerLimit
  レールの動力がどこまで動力を伝達できるかを設定する。1から1024までの整数値をとる。
  + 初期値 : `9`
  + 使用できる値 : `integer`
### renewableBlackstone
　溶岩流が青氷に流れるときブラックストーンを生成する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### renewableCoral
  サンゴに骨粉を与えることでサンゴブロック(ストラクチャー)になるようにする。`expanded`にするとウチワサンゴでも可能になる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `expanded`
### renewableDeepslate
　通常の丸石製造機がy0以下で深層岩を生成する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### renewableSponges
  ガーディアンが雷に打たれるとエルダーガーディアンになるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### rotatorBlock
  サボテンのはいったディスペンサーの正面に方向のあるブロックがあると、トリガーされたときに正面のブロックの方向を変える。ほかのアイテムがはいっているときはそちらが優先され、確率も含めサボテンは無視される。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [flippinCactus](#flippincactus)
### scriptsAppStore
  scriptをゲーム内でダウンロードするさいの場所を指定する。コンソールにおける`cd`に同じ。github上の有効なパブリックリポジトリのリンクのみ受け付ける。`none`とした場合無効になる。
  + 初期値 : `gnembon/scarpet/contents/programs`
  + 使用できる値 : `string`
  + 関連項目
    + [commandScript](#commandscript)
    + script
### scriptsAutoload
  `/script`が有効になっている場合、serverがリスタートもしくはワールドが読み込まれたときに自動的に読み込まれるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [commandScript](#commandscript)
    + script
### scriptsDebugging
  スクリプトのデバッグメッセージを表示するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` 
  + 関連項目
    + [commandScript](#commandscript)
    + script 
### scriptsOptimization
  スクリプトを最適化する。
  
  **一部正常に起動しなくなるスクリプトがあることに注意。**
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [commandScript](#commandscript)
    + script
### sculkSensorRange
  スカルくセンサーの振動を伝える半径を変更する。1から1024の整数値である必要がある。
  + 初期値 : `8`
  + 使用できる値 : `integer`
### shulkerSpawningInEndCities
  シュルカーがエンドシティーでリスポーンするようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### silverFishDropGravel
  シルバーフィッシュがブロックから抜け出すときに砂利をドロップするようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### simulationDistance
  サーバーのシミュレーション距離をこの値でオーバーライドする。0から32の間である必要があり、`0`にすると無効になる。  
  + 初期値 : `0`
  + 使用できる値 : `integer`
  + 関連項目
    + [viewDistance](#viewdistance)
### smoothClientAnimations
  低いtpsでアニメーションをスムーズにする。さらにシングルプレイではtpsにあわせてプレイヤーの飛行速度が変動するようになる。
  
  **クライアントのみ**
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### spawnChunksSize
  スポーンチャンクの半径を指定する。`0`にするとスポーンチャンクを無効にできる。
  + 初期値 : `11`
  + 使用できる値 : `integer`
### stackableShulkerBoxes
  中身のはいっていないシュルカーを地面になげたとき重ねることができる。2から64までの数値または`true` `false`のみを受け付ける。`true`にすると64になる。
  + 初期値 : `false`
  + 使用できる値 : `string`
### structureBlockIgnored
  ストラクチャーブロックが無視するブロックのidを指定する。複数指定することはできない。
  + 初期値 : `minecraft:structure_void`
  + 使用できる値 : `string`
  + 関連項目
    + [structureBlockLimit](#structureblocklimit)
    + [structureBlockOutlineDistance](#structureblockoutlinedistance)
### structureBlockLimit
  各軸に対するストラクチャーブロックのサイズ制限を変更する。値は48以上でなければならない。  
  >[!note]
  >値が大きい場合、負荷軽減の目的で[structureBlockIgnored](#structureblockignored)をminecraft:airにすることを推奨。

  >[!note]
  >ストラクチャーブロックが常に読み込まれていなければ正しく動かない。
  + 初期値 : `48`
  + 使用できる値 : `integer`
  + 関連項目
    + [structureBlockIgnored](#structureblockignored)
    + [structureBlockOutlineDistance](#structureblockoutlinedistance)
### structureBlockOutlineDistance
  ストラクチャーブロックのアウトラインを視認できる距離を変更する。値は非負整数でなければならない。
  
  **クライアントのみ**
  + 初期値 : `96`
  + 使用できる値 : `integer`
  + 関連項目
    + [structureBlockIgnored](#structureblockignored)
    + [structureBlockLimit](#structureblocklimit)
### summonNaturalLightning
  `/summon lightning_bolt`で召喚した稲妻が自然発生した稲妻と同様の効果を与えるようにする。帯電化や炎上など。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### superSecretSetting
  u306Au3093u3082u308Fu304Bu3089u306Au3044u308821
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### thickFungusGrowth
  ネザーの菌類を3x3のベースがあるときに太いネザーの菌糸に成長するようにする。　　
  `false`で無効に、`random`で6%の確率で太く、`all`で条件を満たしていればすべて太くなる。
  + 初期値 : `false`
  + 使用できる値 : `false` `random` `all`
### tickSyncedWorldBorders
  ワールドボーダーの見た目の移動が現実時間ではなくtickをもとにするようにする。これによりtpsを変更するとそれに従って見た目上のスピードが変わるようになる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tntDoNotUpdate
  tntが動力源のとなりに置かれたときに自身をupdateしなくする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tntPrimerMomentumRemoved
  着火によるtntの横方向のランダムなモーメントを0にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tntRandomRange
  tntの爆発範囲をこの値に設定する。-1.0を除いて正の数でなければならない
  >[!important]
  >[optimizedTNT](#optimizedtnt)を有効にする必要がある。
  + 初期値 : `-1.0`
  + 使用できる値 : `double`
### updateSuppressionBlock
  アクティベータレールをバリアブロックの上に置くと、レールがオフになったときに`neighor update stack`が埋められる。この値はスタックに残すべき更新の量。
  + 初期値 : `-1`
  + 使用できる値 : `integer`
### viewDistance
  サーバーの描画距離をこの値でオーバーライドする。0から32の間である必要があり、`0`にすると無効になる。  
  + 初期値 : `0`
  + 使用できる値 : `integer`
  + 関連項目
    + [simulationDistance](#simulationdistance)
### xpFromExplosions
  xpをドロップするブロックはどんな爆発からでもxpをドロップするようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### xpNoCooldown
  xpの吸収のクールダウンを消すことができる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

## counter
  `/counter <color> <realtime | reset>` <br>
  で使用する。ホッパーが羊毛を向くように設置されているとき、そのホッパーが回収したアイテムと有効になっている時間をカウントし、それらから効率を計算する。複数のホッパーを同じチャンネルで作動させることも可能。羊毛16色を用いて16チャンネルを同時に使うことができる。
  + `<color>` <br>
    割愛。複数選択はできない。
  + `<realtime | reset>`
    + `realtime` <br>
      リアルタイムでの効率を計測する。このフラグをつけない場合、tpsが20以外になるとデフォルトの単位時間が72000gtなので実際の1hの効率ではなくなる。このフラグによってそれを是正し、実際の1hの効率を求めることができる。
    + `reset` <br>
      指定したチャンネルもしくは指定しなかった場合すべてのチャンネルの計測をリセットする。
  + 関連項目
    + [hopperCounters](#hoppercounters)

## distance
`/distance <from> <to>`<br>
で`<from>`から`<to>`までの距離を複数の方法で測ることができる。
+ `<from>`<br>
  距離の始点を指定する。絶対座標、チルダ表記法、キャレット表記法の全てを使うことができる。座標を指定しなかった場合`~ ~ ~`が補われる。
+ `<to>`<br>
  距離の終点を指定する。絶対座標、チルダ表記法、キャレット表記法の全てを使うことができる。座標を指定しなかった場合`~ ~ ~`が補われる。

  >[!note]
  >`<from>`のみを入力した場合、その座標を保存して次回のコマンド使用時の始点として利用できる。

+ 実行結果<br>
  正しく計算されると三つの値が生成される。ただし計算には入力された座標を小数第二位までに丸めて使用され、出力は小数第一位までとなる。
  + `Spherical`<br>
    ユークリッド距離で算出。
    始点を$P_1(x_1,y_1,z_1)$、終点を$P_2(x_2,y_2,z_2)$とすると距離$d_m(P_1,P_2)$は
    $$d_E(P_1 , P_2)\coloneqq\sqrt{(x_1-x_2)^2+(y_1-y_2)^2+(z_1-z_2)^2}$$
    >[!note]
    >minecraftではほとんどがユークリッド距離を利用している。`CanSpawnArea`もユークリッド距離である。
  + `Cyrindrical`<br>
    $x$座標および$z$座標のみを用いてユークリッド距離で算出。
    $$d_C(P_1 , P_2)\coloneqq\sqrt{(x_1-x_2)^2+(z_1-z_2)^2}$$
  + `Manhattan`<br>
    マンハッタン距離で算出。
    $$d_M(P_1 , P_2)\coloneqq|x_1-x_2|+|y_1-y_2|+|z_1-z_2|$$
+ 関連項目
  + [commandDistance](#commanddistance)