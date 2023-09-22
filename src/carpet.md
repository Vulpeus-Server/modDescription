# carpet
version : carpet 1.4.1.12+v230608

このドキュメント内では
`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はcarpetおよびそのaddonで日本語ドキュメントが存在もしくは作られる予定のリストである。

|mod|download|document|docs-JP|
|:---:|:---:|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|here|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|[TIS](/carpet-TIS-addition.html)|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)||
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](/gugle-carpet-addition.html)|



## 目次
<details>
  <summary>general</summary>

  + [carpet](#carpet-1)
</details>

<details>
  <summary>rules</summary>

  + [allowSpawningOfflinePlayers](#allowspawningofflineplayers)
  + [antiCheatDisabled](#anticheatdisabled)
  + [carpetCommandPermissionLevel](#carpetcommandpermissionlevel)
  + [carpets](#carpets)
  + [chainStone](#chainstone)
  + [cleanLog](#cleanlog)
  + [commandDistance](#commanddistance)
  + [commandDraw](#commandDraw)
  + [commandInfo](#commandInfo)
  + [commandLog](#commandLog)
  + [commandPerimeterInfo](#commandperimeterinfo)
  + [commandPlayer](#commandplayer)
  + [commandProfile](#commandprofile)
  + [commandScript](#commandscript)
  + [commandScriptACE](#commandscriptace)
  + [commandSpawn](#commandspawn)
  + [commandTick](#commandtick)
  + [commandTrackingAI](#commandtrackingai)
  + [creativeFlyDrag](#creativeflydrag)
  + [creativeFlySpeed](#creativeflyspeed)
  + [creativeNoClip](#creativenoclip)
  + [creativePlayersLoadChunks](#creativeplayersloadchunks)
  + [ctrlQCraftingFix](#ctrlqcraftingfix)
  + [customMOTD](#custommotd)
  + [defaultLoggers](#defaultloggers)
  + [desertShrubs](#desertshrubs)
  + [explosionNoBlockDamage](#explosionnoblockdamage)
  + [fastRedstoneDust](#fastredstonedust)
  + [fillLimit](#filllimit)
  + [fillUpdates](#fillupdates)
  + [flippinCactus](#flippincactus)
  + [fogOff](#fogoff)
  + [forceloadLimit](#forceloadlimit)
  + [hardcodeTNTangle](#hardcodetntangle)
  + [hopperCounters](#hoppercounters)
  + [huskSpawningInTemples](#huskspawningintemples)
  + [interactionUpdates](#interactionupdates)
  + [lagFreeSpawning](#lagfreespawning)
  + [lightningKillsDropsFix](#lightningkillsdropsfix)
  + [liquidDamageDisabled](#liquiddamagedisabled)
  + [maxEntityCollisions](#maxentitycollisions)
  + [mergeTNT](#mergetnt)
  + [missingTools](#missingtools)
  + [moreBlueSkulls](#moreblueskulls)
  + [movableAmethyst](#movableamethyst)
  + [movableBlockEntities](#movableblockentities)
  + [optimizedTNT](#optimizedtnt)
  + [perfPermissionLevel](#perfpermissionlevel)
  + [persistentParrots](#persistentparrots)
  + [piglinsSpawningInBastions](#piglinsspawninginbastions)
  + [pingPlayerListLimit](#pingplayerlistlimit)
  + [placementRotationFix](#placementrotationfix)
  + [portalCreativeDelay](#portalcreativedelay)
  + [portalSurvivalDelay](#portalsurvivaldelay)
  + [pushLimit](#pushlimit)
  + [quasiConnectivity](#quasiconnectivity)
  + [railPowerLimit](#railpowerlimit)
  + [renewableBlackstone](#renewableblackstone)
  + [renewableCoral](#renewablecoral)
  + [renewableDeepslate](#renewabledeepslate)
  + [renewableSponges](#renewablesponges)
  + [rotatorBlock](#rotatorblock)
  + [scriptsAppStore](#scriptsappstore)
  + [scriptsAutoload](#scriptsautoload)
  + [scriptsDebugging](#scriptsdebugging)
  + [scriptsOptimization](#scriptsoptimization)
  + [sculkSensorRange](#sculksensorrange)
  + [shulkerSpawningInEndCities](#shulkerspawninginendcities)
  + [silverFishDropGravel](#silverfishdropgravel)
  + [simulationDistance](#simulationdistance)
  + [smoothClientAnimations](#smoothclientanimations)
  + [spawnChunksSize](#spawnchunkssize)
  + [stackableShulkerBoxes](#stackableshulkerboxes)
  + [structureBlockIgnored](#structureblockignored)
  + [structureBlockLimit](#structureblocklimit)
  + [structureBlockOutlineDistance](#structureblockoutlinedistance)
  + [summonNaturalLightning](#summonnaturallightning)
  + [superSecretSetting](#supersecretsetting)
  + [thickFungusGrowth](#thickfungusgrowth)
  + [tickSyncedWorldBorders](#ticksyncedworldborders)
  + [tntDoNotUpdate](#tntdonotupdate)
  + [tntPrimerMomentumRemoved](#tntprimermomentumremoved)
  + [tntRandomRange](#tntrandomrange)
  + [updateSuppressionBlock](#updatesuppressionblock)
  + [viewDistance](#viewdistance)
  + [xpFromExplosions](#xpfromexplosions)
  + [xpNoCooldown](#xpnocooldown)
</details>

<details>
<summary>command</summary>

  + [counter](#counter)
  + [distance](#distance)
  + [draw](#draw)
  + [info](#info)
  + [log](#log)
  + [perimeterInfo](#perimeterinfo)
  + [profile](#profile)
  + [player](#player)
  + [script](#script)
  + [spawn](#spawn-1)
  + [tick](#tick)
  + [track](#track)

</details>


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
    <div class="md-note">
    
      `/carpet [rule] [value]`を使用し値が正常に変更された場合、通知とともにそえられる`change permanently?`を右クリックすることでその値がすでに入力されたコマンドが準備される。
    </div>

  + `/carpet removeDefault <rule>`<br>
    `[rule]`で指定したcarpet ruleのデフォルトの値を`carpet.conf`から削除し、初期値にする。

## rules
全てのルールは`/carpet [rule] <value>`によって変更することができる。
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
  <div class="md-note">
    現在たいち鯖では最大のパーミッションレベルが3になっている。
  </div>

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
    + [info](#info)
    + [spawn](#spawn-1)
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
    + [draw](#draw)
### commandInfo
  `/info`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [info](#info)
### commandLog
  `/log`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [log](#log)
### commandPerimeterInfo
  `/perimeterinfo`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [perimeterInfo](#perimeterinfo)
### commandPlayer
  `/player`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [player](#player)
### commandProfile
  `/profile`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [profile](#profile)
### commandScript
  `/script`のscript作成を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [script](#script)
### commandScriptACE
  `/script load` `/script run`を使用できるプレイヤーを指定する。appが実行するときのopレベルでもある。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [script](#script)
### commandSpawn
  `/spawn`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [spawn](#spawn-1)
### commandTick
  `/tick`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [tick](#tick)
### commandTrackingAI
  `/track`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [track](#track)
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
  クライアントとサーバーの双方に設定があるため、同じ設定にしないと動作が不安定になる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### creativePlayersLoadChunks
  クリエイティブのプレイヤーが周囲のチャンクをロードするかを設定する。
  <div class="md-note">
  
  スペクテイターモードについては`/gamerule spectatorsGenerateChunks`によって設定可能。
  </div>

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
  サーバーに入ったときに表示するログの初期値。ただしsetDefaultを設定しないと再起動によって初期値に戻る。
  `tps,mobcaps,counter`のように、カンマで常げることでサジェストされたもの以外も指定できる。
  + 初期値 : `none`
  + 使用できる値 : `string`
  + 関連項目
    + [log](#log)
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
  <div class="md-note">
  壊れる回路があるので注意。
  </div>

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
    + TIS / [totallyNoBlockUpdate](/carpet-TIS-addition.html#totallynoblockupdate)
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
  `/counter`を有効にする。詳しくは[counter](#counter)を参照。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [counter](#counters)
    + TIS / [hopperCountersUnlimitedSpeed](/carpet-TIS-addition.html#hoppercountersunlimitedspeed)
    + TIS / [hopperNoItemCost](/carpet-TIS-addition.html#hoppernoitemcost)
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
  + 関連項目
    + TIS / [optimizedTNTHighPriority](/carpet-TIS-addition.html#optimizedtnthighpriority)
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
    + [script](#script)
### scriptsAutoload
  `/script`が有効になっている場合、serverがリスタートもしくはワールドが読み込まれたときに自動的に読み込まれるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [commandScript](#commandscript)
    + [script](#script)
### scriptsDebugging
  スクリプトのデバッグメッセージを表示するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` 
  + 関連項目
    + [commandScript](#commandscript)
    + [script](#script) 
### scriptsOptimization
  スクリプトを最適化する。
  
  **一部正常に起動しなくなるスクリプトがあることに注意。**
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [commandScript](#commandscript)
    + [script](#script)
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
  <div class="md-note">

  値が大きい場合、負荷軽減の目的で[structureBlockIgnored](#structureblockignored)をminecraft:airにすることを推奨。
  </div>
  <div class="md-note">

  >ストラクチャーブロックが常に読み込まれていなければ正しく動かない。
  </div>
  
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
  <div class="md-important">

  [optimizedTNT](#optimizedtnt)を有効にする必要がある。
  </div>

  + 初期値 : `-1.0`
  + 使用できる値 : `double`
### updateSuppressionBlock
  アクティベータレールをバリアブロックの上に置くと、レールがオフになったときに`neighor update stack`が埋められる。この値はスタックに残すべき更新の量。
  + 初期値 : `-1`
  + 使用できる値 : `integer`
  + 関連項目
    + TIS / [updateSuppressionSimulator](/carpet-TIS-addition.html#updatesuppressionsimulator)
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

## command
### counter
  `/counter <color> <realtime | reset>` <br>
  で使用する。ホッパーが羊毛を向くように設置されているとき、そのホッパーが回収したアイテムと有効になっている時間をカウントし、それらから効率を計算する。複数のホッパーを同じチャンネルで作動させることも可能。羊毛16色を用いて16チャンネルを同時に使うことができる。
  + `<color>` <br>
    割愛。複数選択はできない。選択しなかった場合すべての有効なチャンネルを表示する。
  + `<realtime | reset>`
    + `realtime` <br>
      リアルタイムでの効率を計測する。このフラグをつけない場合、tpsが20以外になるとデフォルトの単位時間が72000gtなので実際の1hの効率ではなくなる。このフラグによってそれを是正し、実際の1hの効率を求めることができる。
    + `reset` <br>
      指定したチャンネルもしくは指定しなかった場合すべてのチャンネルの計測をリセットする。
  + 関連項目
    + [hopperCounters](#hoppercounters)

### distance
`/distance <from> <to>`<br>
で`<from>`から`<to>`までの距離を複数の方法で測ることができる。
+ `<from>`<br>
  距離の始点を指定する。絶対座標、チルダ表記法、キャレット表記法の全てを使うことができる。座標を指定しなかった場合`~ ~ ~`が補われる。
+ `<to>`<br>
  距離の終点を指定する。絶対座標、チルダ表記法、キャレット表記法の全てを使うことができる。座標を指定しなかった場合`~ ~ ~`が補われる。

  <div class="md-note">

  `<from>`のみを入力した場合、その座標を保存して次回のコマンド使用時の始点として利用できる。
  </div>

+ 実行結果<br>
  正しく計算されると三つの距離空間に基づく値が表示される。ただし計算には入力された座標を小数第二位までに丸めて使用され、出力は小数第一位までとなる。

  <details>
  <summary>距離空間と定義</summary>

  + `Spherical`<br>
    ユークリッド距離で算出。
    始点を \\( P_1(x_1,y_1,z_1) \\)、終点を \\( P_2(x_2,y_2,z_2) \\)とすると距離 \\( d_S(P_1,P_2) \\) は
    $$d_S(P_1 , P_2) := \sqrt{(x_1-x_2)^2+(y_1-y_2)^2+(z_1-z_2)^2}$$

  + `Cyrindrical`<br>
     \\( x \\) 座標および  \\( z \\) 座標のみを用いてユークリッド距離で算出。
    $$d_C(P_1 , P_2) := \sqrt{(x_1-x_2)^2+(z_1-z_2)^2}$$
  + `Manhattan`<br>
    マンハッタン距離で算出。
    $$d_M(P_1 , P_2) := |x_1-x_2|+|y_1-y_2|+|z_1-z_2|$$
  
  <div class="md-note">

  minecraftではほとんどがユークリッド距離を利用している。`CanSpawnArea`もユークリッド距離である。
  </div>

  </details>
+ 関連項目
  + [commandDistance](#commanddistance)

### draw
`/draw [shape] [coordinate]`で利用可能。`[shape]`の図形を生成できる。ときにはWorldEditに負ける。ほとんどにおいてWorldEditで代替可能であるが、diamondやconeなどはこれでつくったほうが　はやいだろう。
+ `[shape]`
  + [ball](#ball)
  + [cone](#cone)
  + [cuboid](#cuboid)
  + [cylinder](#cylinder)
  + [diamond](#diamond)
  + [pyramid](#pyramid)
  + [sphere](#sphere)
+ 関連項目
  + [commandDraw](#commanddraw)
<details>
  <summary>詳細</summary>

#### ball
  中が満たされた球体を生成する。
  `/draw ball [center] [radius] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物、ここでは球体の中心となる座標を指定する。絶対座標と相対座標のどちらも使うことができる。小数で入力した場合その座標を含むブロックの座標が選択される。
  + `[radius]`<br>
    半径を指定する。値は0より大きい整数でなければならない。
  + `[block]`<br>
    描くブロックを指定する。WorldEditのように複数をランダムに指定することはできない。
    <div class="md-important">
    あとからWorldEdit等を用いることで割合指定でランダムに変更することができる。
    </div>

  + `<replace>`<br>
    特定のブロック***を***置き換えるかを指定する。指定しなかった場合全てのブロックを置き換える。
  + 関連項目
    + [draw sphere](#sphere)
#### cone
  中が満たされた円柱を生成する。
  `/draw cone [center] [radius] [height] [pointing] [axis] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物の底面の中心となる座標を指定する。
  + `[radius]`<br>
    底面の半径を指定する。
  + `[height]`<br>
    生成物の高さを指定する。
  + `[pointing]`
    + `down`<br>
      先端が`[axis]`の座標マイナス方向を向く。
    + `up`<br>
      先端が`[axis]`の座標プラス方向を向く。
  + `[axis]`<br>
    生成物がx軸を基準とする。
    + `x`
    + `y`
    + `z`
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック**を**置き換えるかを指定する。
#### cuboid
  中が満たされた四角柱を生成する。
  `/draw cuboid [center] [radius] [height] [pointing] [axis] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物の底面の中心となる座標を指定する。
  + `[radius]`<br>
    底面の一辺の長さを指定する。
    <div class="md-note">
    この値を半径とする円に外接し、一辺が各軸にそうような正方形が底面となる。
    </div>

  + `[height]`<br>
    生成物の高さを指定する。
  + `[pointing]`
    + `down`<br>
      先端が`[axis]`の座標マイナス方向を向く。
    + `up`<br>
      先端が`[axis]`の座標プラス方向を向く。
  + `[axis]`<br>
    生成物がその軸を中心にする。
    + `x`
    + `y`
    + `z`
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック**を**置き換えるかを指定する。
#### cylinder
  中が満たされた円柱を生成する。
  `/draw cylinder [center] [radius] [height] [pointing] [axis] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物の中心となる座標を指定する。
  + `[radius]`<br>
    底面の半径を指定する。
  + `[height]`<br>
    生成物の高さを指定する。
  + `[pointing]`<br>
    + `down`<br>
    `[axis]`の座標の負の方向に生成する。
    + `up`<br>
    `[axis]`の座標の正の方向に生成する。
  + `[axis]`<br>
    + `x`
    + `y`
    + `z`
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック***を***置き換えるかを指定する。
#### diamond
  中空の正八面体を生成する。
  `/draw diamond [center] [radius] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物の中心となる座標を指定する。
  + `[radius]`<br>
    中心からの最大距離を指定する。
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック***を***置き換えるかを指定する。
#### pyramid
  中が満たされた円柱を生成する。
  `/draw pyramid [center] [radius] [height] [pointing] [axis] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    生成物の中心となる座標を指定する。
  + `[radius]`<br>
    底面の一辺の長さを指定する。
    <div class="md-important">
    この値を半径とする円に外接し、一辺が各軸にそうような正方形が底面となる。
    </div>
  + `[height]`<br>
    生成物の高さを指定する。
  + `[pointing]`<br>
    + `down`<br>
    `[axis]`の座標の負の方向に生成する。
    + `up`<br>
    `[axis]`の座標の正の方向に生成する。
  + `[axis]`<br>
    + `x`
    + `y`
    + `z`
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック***を***置き換えるかを指定する。
#### sphere
  中空の球体を生成する。
  `/draw sphere [center] [radius] [block] <replace>`<br>
  で利用可能。
  + `[center]`<br>
    球体の中心となる座標を指定する。
  + `[radius]`<br>
    半径を指定する。
  + `[block]`<br>
    描くブロックを指定する。
  + `<replace>`<br>
    特定のブロック**を**置き換えるかを指定する。
  + 関連項目
    + [draw ball](#ball)

</details>

### info
指定した情報を表示する。opレベル0を要求する。WorldEditによって完全に代替される予定であるとのこと。
`/info [block | entity] [target] <grep>`
で実行可能。`<grep>`によって表示する情報を制限することが可能。
+ `[block | entity]`
  + `block`<br>
    `[target]`は表示したいブロックの座標となる。絶対座標もしくは相対座標を使うことができる。
  + `entity`<br>
    `[target]`は表示したいエンティティとなる。一つのエンティティのみを選択する必要がある。
    <div class="md-note">

    ターゲットセレクタで指定する場合`[limit=1]`と追記することで一つのエンティティに絞ることができる。
    </div>

+ 関連項目
  + [commandInfo](#commandinfo)

### log
`/log [subject] <mcid>`で`[subject]`に関する情報をさまざまなところに表示する。
+ `[subject]`
  + `counter`
  + `fallingBlocks`
  + `mobcaps`
  + `packets`
  + `pathfinding`
  + `projectiles`
  + `tnt`
  + `tps`
+ `/log clear`<br>
  全てのlogの表示を停止させることができる。
  <div class="md-note">
  
  `/log [subject] clear`とすることでそのlog表示を消すことができる。
  </div>

+ `<mcid>`<br>
  指定することでその人に表示させることができる。
+ 関連項目
  + [commandLog](#commandlog)
  + [defaultLoggers](#defaultloggers)
<details>
  <summary>subject</summary>
  
  #### `counter`
  `/log counter <color> <mcid>`で利用可能。特定のチャンネルに対して収集されたアイテム数とその効率、計測時間を表示する。
  + `<color | clear>`<br>
    チャンネルを指定する。指定しなかった場合`white`もしくはそれが無効であるならばほかの有効なチャンネルが選択される。さらに有効なチャンネルが一切ない場合は`white`が表示される。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + [counter](#counter)
  #### `fallingBlocks`
  `/log fallingBlocks <brief | full> <mcid>`で利用可能。falling blockの生成時のtickから消失時のtickまで、各tickの正確な座標とそれぞれのモーメントを表示する。
  + `<brief | full>`<br>
    表現の方法を指定する。指定しなかった場合`brief`が指定される。
    + `brief`<br>
      省略して表示する。ホバーすることで正確な情報が得られる。
    + `full`<br>
      省略せずにすべてを表示する。
  + 表示場所<br>
    チャット
  #### `mobcaps`
  `/log mobcaps <dimension | dynamic> <mcid>`で利用可能。指定したディメンションのmobcapを表示する。
  + `<dimension | dynamic>`<br>
  そのディメンションにおけるmobcapを表示する。指定しないと`dynamic`が指定される。
    + `dimension`<br>
      そのディメンションにおけるmobcapを表示する。カスタムディメンションをdatapack等であらたに作成した場合そのディメンションidが入力できるようになる。
    + `dynamic`<br>
      自身のいるディメンションが自動的に選択され、ディメンションを移動すると表示されるディメンションも変わる。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + spawn
  #### `packets`
  `/log packets <mcid>`で利用可能。通信時のパケット量を単位を/sとして表示する.。Iがサーバーへ、Oがクライアントへのパケット量。
  + 表示場所<br>
    プレイヤーリスト
  #### `pathfinding`
  `/log pathfinding [count] <mcid>`で利用可能。pathfindingは行動探索であるが、どういった挙動を示すかは不明。
  + `[count]`<br>
    おそらくlogに流すentityの量。
  + 表示場所<br>
    わがらん
  #### `projectiles`
  `/log projectiles <brief | full> <mcid>`で利用可能。飛び道具、主にポーションや矢のentity生成時のtickから消失時のtickまで、各tickの正確な座標とそれぞれのモーメントを表示する。当たったとき、その座標も表示する。
  + `<brief | full>`<br>
    表現の方法を指定する。指定しなかった場合`brief`が指定される。
    + `brief`<br>
      省略して表示する。ホバーすることで正確な情報が得られる。
    + `full`<br>
      省略せずにすべてを表示する。
  + 表示場所<br>
    チャット
  #### `tnt`
  `/log tnt <brief | full> <mcid>`で利用可能。tntがいつ、どこで、誰によって、どのようにして、ベクトルの始点がどこであるかを表示する。
  + `<brief | full>`<br>
    表現の方法を指定する。指定しなかった場合`brief`が指定される。
    + `brief`<br>
      省略して表示する。ホバーすることで正確な情報が得られる。
    + `full`<br>
      省略せずにすべてを表示する。値がより詳細になる。
  + 表示場所<br>
    チャット
  #### `tps`
  `/log tps <mcid>`で利用可能。tpsとmsptを表示する。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + tick

</details>

### perimeterInfo
`/perimeterinfo <coordinate>　<mob>`で利用可能。perimeterについて湧くことが可能なブロックを表示する。
+ `<coordinate>`<br>
  perimeterの中心、プレイヤーが立つ座標を入力する。この座標を中心に半径128ブロ空の球体内に関して表示する。指定しなかった場合現在の座標`~ ~ ~`が指定される。
+ `<mob>`<br>
  この`<mob>`が湧くことができるブロックを表示するようにする。指定しなかった場合すべての存在するmobが指定される。
+ 関連項目
  + [commandPerimeterInfo](#commandperimeterinfo)

### profile
`/profile [entities | health]`で`/tick <entities | health>`と同様の働きをする。詳しくは[tick](#tick)を参照。
+ 関連項目
  + [commandProfile](#commandprofile)
  + [tick](#tick)

### player
  `/player [mcid] [action]`で様々なプレイヤーに関する操作を行える。
  + `[action]`
    + `attack`
    + `dismount`
    + `drop`
    + `dropStack`
    + `hotbar`
    + `jump`
    + `kill`
    + `look`
    + `mount`
    + `move`
    + `shadow`
    + `sneak`
    + `spawn`
    + `sprint`
    + `stop`
    + `swapHands`
    + `turn`
    + `unsneak`
    + `unsprint`
    + `use`
  + 関連項目
    + [commandPlayer](#commandplayer)

<details>
  <summary>action</summary>

#### attack
  なにも指定しなかった場合、`once`が指定される。
  + continuous<br>
    `/player [mcid] attack continuous`<br>
    連続的に攻撃させる。
  + interval<br>
    `/player [mcid] attack interval [count]`<br>
    `[counter]`gt毎に攻撃させる。
  + once<br>
    `/player [mcid] attack once`<br>
    一回だけ攻撃させる。
#### dismount
  現在乗っているエンティティから降ろさせる。なににものっていなかった場合なにもおきない。<br>
  `/player [mcid] dismount`
#### drop
  今メインハンドにもっているものを一つその場に落とさせる。<br>
  `/player [mcid] drop`
#### dropStack
  今メインハンドにもっているものを1スタックその場に落させる。<br>
  `/player [mcid] dropStack`
#### hotbar
  今手にもっているスロットを変更させる。<br>
  `/player [mcid] hotbar [number]`
#### jump
  その場でジャンプさせる。<br>
  `/player [mcid] jump`
#### kill
  対象をkillする。<br>
  `/player [mcid] kill`
#### look
  特定の方向を向かせる。<br>
  `/player [mcid] look [[pitch yaw] | up | down | north | south | east | west | at [x y z]]`
  + `[pitch yaw]`<br>
    ピッチとヨーを指定する。数字はそれぞれ-90から90の間でなければいけない。
  + `up | down | north | south | east | west`<br>
    特定の方向を向かせる。
  + `at [x y z]`<br>
    特定の座標に視線を向かせる。
#### mount
  一番近い乗ることができるエンティティに乗る。よみこまれているエンティティのすべてが乗れない場合、失敗する。<br>
  `/player [mcid] mount`
#### move
  指定された方向へ移動する。
  `/player <name> move [backward | forward | left | right]`
#### shadow
  全ての動作を引き継いで同名のbotを出す。
  `/player [mcid] shadow`
#### sneak
  スニークをさせる。
  `/player [mcid] sneak`
#### spawn
  botとしてplayerを召喚する。
  `/player [mcid] spawn`
#### sprint
  ダッシュさせる。
  `/player [mcid] sprint`
#### stop
  今`[mcid]`に`/player`によって実行されているコマンドを全て停止させる。
  `/player [mcid] stop`
#### swapHands
  オフハンドとメインハンドを入れ替える。
  `/player [mcid] swapHands`
#### turn
  指定した方向を向かせる。
  `/player [mcid] turn [back | left | right]`
#### unsneak
  スニークを解除させる。
  `/player [mcid] unsneak`
#### unsprint

  ダッシュを解除させる。
  `/player [mcid] unsprint`
#### use
  なにも指定しなかった場合、`once`が指定される。
  + continuous<br>
    `/player [mcid] use continuous`<br>
    連続的に使用させる。
  + interval<br>
    `/player [mcid] use interval [count]`<br>
    `[counter]`gt毎に使用させる。
  + once<br>
    `/player [mcid] use once`<br>
    一回だけ使用させる。

</details>

### script
  carpet内で動作するスクリプトを操作する。ゲーム内で作成することができるが、ここでは省略。

### spawn
  `/spawn [subject]`によって実行可能。spawningに関する情報および設定を変更する。
  + `[subject]`
    + `entities`
    + `list`
    + `mobcaps`
    + `mobcapLocal`
    + `rate`
    + `tracking`
  + 関連項目
    + [commandSpawn](#commandspawn)
  <details>
    <summary>subject</summary>

#### `entities`<br>
`/spawn entities <mob_type>`で実行可能。mobcapの占有率や`<mob_type>`を指定した場合そのmob_typeに属するmobの座標を取得できる。
#### `list`<br>
`/spawn list [coordinate]`で実行可能。そのブロックに対して理論上湧くことのできるentityを一覧形式で表示する。
#### `mobcaps`<br>
`/spawn mobcaps <dimension>`で実行可能。指定されたdimensionに対するmobcapを表示する。
#### `mobcapLocal`<br>
`/spawn mobcapLocal [selector]`で実行可能。プレイヤーの周りに発生するmobcapを計測する。
#### `rate`<br>
`/spawn rate [mob_type] [round]`で実行可能。`[mob_type]`の1tickに試行されるspawning回数を`[round]`の値に変更する。
#### `tracking`<br>
`/spawn tracking [mob_type | action]`で実行可能。`[mob_type]`のspawn回数やspawn率を表示す。 
  </details>

### tick
`/tick [action]`によりminecraftのtickに関する制御をする。
+ `[action]`
  + `entities`
  + `freeze`
  + `health`
  + `rate`
  + `step`
  + `superHot`
  + `warp`
+ 関連項目
  + [commandTick](#commandtick)

<details>
   <summary>action</summary>

  #### entities
  `/tick entities <tick>`で実行可能。`<tick>`gtの間entityの量や種類などを計算し、その上位を表示する。指定しなかった場合300gtで計算する。
  #### freeze
  `/tick freeze <true | false | deep | status>`で実行可能。`true`もしくは`false`を選択することで現在のtickで停止もしくは再開させることができる。`status`は現在freezeしているかの確認ができ、`deep`ではより深いタイミングでのfreezeを可能にする。指定しなかった場合trueとfalseがトグルとなる。
  #### health
  `/tick health <tick>`で実行可能。`<tick>`gtの間どの処理が負荷となっているかを計測し、その上位を表示する。指定しなかった場合300gtで計測する。
  #### rate
  `/tick rate [count]`で実行可能。現在のtick rateを`[count]`の値にする。ただしtickはmsptに基づいて計算されるため正確な値が反映されるわけではないことに注意。
  #### step
  freeze中に`\tick step [count]`で実行可能。`[count]`の数だけtickを進める。
  #### superHot
  `/tick superHot [true | false]`で実行可能。プレイヤーが移動するまでtickがfreezeするsuperHotモードを有効にできる。ゲーム「super hot」から。
  #### warp
  `/tick warp [count]`で実行可能。最適化をしたうえでできるだけ最速で`[count]`の数字分だけ早送りしようとする。

</details>

### track
`/track [entity_type] [tracker]`で実行可能。ただしscriptなしでは`[entity_type]`はvillagerのみとなっている。`[tracker]`によって表示するtracking情報はことなるが多いので割愛。
