# carpet

このドキュメント内では
`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

[carpet公式ドキュメント](https://github.com/gnembon/fabric-carpet/wiki/Current-Available-Settings)

## 目次
<details>
  <summary>
    + general
      <summary>
        + /carpet
      </summary>
      /carpet list
  </summary>
</details>

+ general
+ rule
+ counter
+ tick
+ player
+ profile
+ log
+ info
+ distance
+ draw
+ spawn
+ perimeterinfo
+ script

## general
### `/carpet`
現在変更されているcarpetの設定、導入されているcarpetのバージョン、カテゴリーを表示する。
### `/carpet list <category>`
利用できるcarpet ruleを**すべて**表示する。`<category>`を指定した場合、紐づけられたruleを表示する。
### `/carpet list defaults`
`carpet.conf`に記録されているルールを表示する。
### `/carpet setDeffault [rule] [value]`
`[rule]`で指定したcarpet ruleのデフォルトの値を`[value]`で指定した値にする。  
`/carpet [rule] [value]`を使用し値が正常に変更された知らせとともに通知される`change permanently?`を右クリックすることでその値がすでに入力されたコマンドが設定される。
### `/carpet rmeoveDeffault [rule]`
`[rule]`で指定したcarpet ruleのデフォルトの値を`carpet.conf`から削除し、初期値にする。


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

## rule
`/carpet [rule] <value>`によって変更することができる。
### ~allowSpawningOfflinePlayers~
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  オフラインのプレイヤーを召喚できるかを設定できる。
  オフラインのプレイヤーは`/player [mcid] [spawn | shadow]`によるものではないことを確認。
### antiCheatDisabled
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  バニラ標準のアンチチートを無効化する。アンチチートにはプレイヤーのリーチ制限や移動量制限などが含まれ、それぞれが数値上の最大値まで許容することができるようになる。
### carpetCommandPermissionLevel
  + 初期値 : `ops`
  + 使用できる値 : `ops` `2` `4`

  `/carpet`コマンドを使用できるパーミッションレベルを指定する。`ops`では`/op`で付与された人のみであるが、`2` `4`はそれぞれの数値以上のパーミッションを保持しているプレイヤーにが使うことができる。

  現在たいち鯖ではデフォルトのパーミッションレベルは3になっているとのこと。
### carpets
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  carpetを置くことで権限のない人でも特定のコマンドのみ使えるようにする。
  以下は使用できるコマンドのリストである。
  | color  | command                                      |
  |:------:|:---------------------------------------------|
  | gray   | `/info block ~ ~-1 ~`                        |
  | black  | `/spawn entities`                            |
  | brown  | `/distance from ~ ~ ~ ` `/distance to ~ ~ ~` |
  | pink   | `/spawn list ~ ~-1 ~`                        |
### chainStone
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `stick_to_all`

  `chain`を長いほうの端でスライムのように接続でき、かつほかのブロックとも接続できるようにする。`stick_to_all`を指定するとすべての方向について接続する。

### ~cleanLog~
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  クライアントに対するコマンド。どのログがどのように消されるかは謎。

### commandDistance
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/distance`を使用できるプレイヤーを指定する。`true` `false`ではopの所持の如何を問わず指定することができる。

### commandDraw
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/draw`を使用できるプレイヤーを指定する。
  
### commandInfo
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/info`を使用できるプレイヤーを指定する。

### commandLog
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/log`を使用できるプレイヤーを指定する。

### commandPerimeterInfo
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/perimeterinfo`を使用できるプレイヤーを指定する。
  
### commandPlayer
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/player`を使用できるプレイヤーを指定する。

### commandProfile
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/profile`を使用できるプレイヤーを指定する。
  
### commandScript
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/script`のscript作成を使用できるプレイヤーを指定する。

### commandScriptACE
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/script load` `/script run`を使用できるプレイヤーを指定する。appが実行するときのopレベルでもある。

### commandSpawn
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/spawn`を使用できるプレイヤーを指定する。

### commandTick
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/tick`を使用できるプレイヤーを指定する。

### commandTrackingAI
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`

  `/track`を使用できるプレイヤーを指定する。

### creativeFlyDrag
  + 初期値 : `0.09`
  + 使用できる値 : `double`

  クリエイティブにおける空気抵抗(慣性の減衰度合い)を設定する。0で一切減衰せず、1でBEのようにストッピングができるようになる。

  **clientのみ**
  
### creativeFlySpeed
  + 初期値 : `1.0`
  + 使用できる値 : `double`

  クリエイティブにおける浮遊時の飛行速度を設定する。
  
  **clientのみ**
  
### reativeNoClip
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  クリエイティブにおける飛行状態でブロックを貫通できるようにする。
  クライアントと鯖の双方に設定があるため、同じ設定にしないと動作が不安定になる。
  
### creativePlayersLoadChunks
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  クリエイティブのプレイヤーが周囲のチャンクをロードするかを設定する。
  スペクテイターモードについては`/gamerule spectatorsGenerateChunks`によって設定可能。

### ctrlQCraftingFix
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  ctrlQによる一括排出をクラフトの結果欄でも機能するようにする。
### ~customMOTD~
  + 初期値 : `_`
  + 使用できる値 : 'string'

  MOTD is なに
### defaultLoggers
  + 初期値 : 'none'
  + 使用できる値 : 'string(defined)'

鯖に入ったときに表示するログの初期値。ただしsetDefaultを設定しないと再起動によって初期値に戻る。

### desertShrubs
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  苗木が砂漠を含めた暑い気候および水のアクセスができない場所で枯れ木にする。

### explosionNoBlockDamage
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  爆発ダメージを起こさなくする。

### fastRedstoneDust
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  redstone dustのupdate orderを複数回更新される場所を一回のみにすることで最適化がされる。**壊れる回路があるので注意。**
  
### fillLimit
  + 初期値 : `32768`
  + 使用できる値 : `integer`

fillやcloneのブロック数制限を変更する。ただしゲームルールに同様の機能があり、そちらの数値に上書きされる。

### fillUpdates
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  fillやclone、setblockによるblock updateを発生させないようにする。

### flippinCactus
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  サボテンをメインハンドに持っている時、方向をもつブロックの一部(たとえばホッパーやオブザーバーなど)を右クリックするとその方向をupdateなしで回転もしくは反転できるようにする。

### fogOff
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  ネザーにおよびエンドにおけるfog(霧)を消すようにする。

  **クライアントのみ**

### forceloadLimit
  + 初期値 : `256`
  + 使用できる値 : `integer`

  forceloadの上限を変更する。
  
### hardcodeTNTangle
  + 初期値 : `-1.0`
  + 使用できる値 : `0 < θ < 2π`

  tntの着火時に起きる水平方向の移動の計算方式を変更する。デフォルトは-1.0であり、これは変更しない(=ランダムである)ことを意味する。使用できる値の範囲内によりその回転を指定できる。

### hopperCounters
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
    
  `/counter`を有効にする。

### huskSpawningInTemples
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  ピラミッドではハスクのみがスポーンできるようにする。

### interactionUpdates
  + 初期値 : `true`
  + 使用できる値 : `true` `false`

  ブロックを置くときにblock updateを発生させないようにする。

### lagFreeSpawning
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  mobのスポーンを最適化する。

### language
  + 初期値 : `en_us`
  + 使用できる値 : `en_us` `fr_fr` `pt_br` `zh_cn` `zh_tw`

  carpetで使用する言語を変更する。

### lightningKillsDropsFix
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

　[MC-206922](https://bugs.mojang.com/browse/MC-206922)を修正する。
 落雷がmobをキルした場合もmobがドロップすべきアイテムをドロップするようにする。

### liquidDamageDisabled
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  流体によるブロックの破壊を起こさなくする。

### maxEntityCollisions
  + 初期値 : `0`
  + 使用できる値 : `interger`

  一つのentityが持つ最大の当たり判定の数。0で無制限。非不整数でなければいけない。

### mergeTNT
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  着火されたtntが同一のfuseを持つ場合それらを起爆したときに同様の爆発ダメージ及びモーメントを与える一つのentityとする。

### missingTools
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  ガラスの適正ツールがつるはしとなる。

### moreBlueSkulls
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  witherによって出される青いskullの確率を上げる。

### movableAmethyst
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

　　芽の生えたアメジストをピストンによって移動できるようにする。また、シルクタッチのついた適正ツールで掘られた場合にはアイテムとしてドロップするようにする。

### movableBlockEntities
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  block entityをピストンにより移動可能にする。
  
### optimizedTNT
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  tntが同じ座標や流体内で爆発したときの最適化をする。

### ~~perfPermissionLevel~~
  + 初期値 : `4`
  + 使用できる値 : `2` `4`

  `/perf`が使用できる権限を変更する。~~しかし`/perf`が確認できなかった。~~

### persistentParrots
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  オウムがダメージをうけるまで常に肩に乗るようにする。

### piglinsSpawningInBastions
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  ピグリン、ピグリンブルート、ホグリンがbastionで自然スポーンすることができるようにする。

### pingPlayerListLimit
  + 初期値 : `12`
  + 使用できる値 : `integer`

  ping playerのサンプル数の上限を設定する。非負整数である必要がある。
  
### placementRotationFix
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  プレイヤーが高速で視点を動かしたときに設置されたブロックが回転するバグを修正する。

### portalCreativeDelay
  + 初期値 : `0`
  + 使用できる値 : `integer`

  プレイヤーがクリエイティブでネザーポータルを通過するために必要な時間を設定する。単位はgtで0から72000までの整数値をとる。

### portalSurvivalDelay
  + 初期値 : `80`
  + 使用できる値 : `integer`

  プレイヤーがサバイバルでネザーポータルを通過するために必要な時間を設定する。単位はgtで0から72000までの整数値をとる。

### pushLimit
  + 初期値 : `12`
  + 使用できる値 : `integer`

  ピストンが押せるブロックの最大量を決める必要がある。1から1024までの整数値をとる。

### quasiConnectivity
  + 初期値 : `true`
  + 使用できる値 : `true` `false`

  ピストンとドロッパー、ディスペンサーの準接続をおこさないようにする。

### railPowerLimit
  + 初期値 : `9`
  + 使用できる値 : `integer`

  レールの動力がどこまで動力を伝達できるかを設定する。1から1024までの整数値をとる。

### renewableBlackstone
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

　溶岩流が青氷に流れるときブラックストーンを生成する。

### renewableCoral
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `expanded`

  サンゴに骨粉を与えることでサンゴブロック(ストラクチャー)になるようにする。`expanded`にするとウチワサンゴでも可能になる。

### renewableDeepslate
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

　通常の丸石製造機がy0以下で深層岩を生成する。

### renewableSponges
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

　ガーディアンが雷に打たれるとエルダーガーディアンになるようにする。

### rotatorBlock
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  サボテンのはいったディスペンサーの正面に方向のあるブロックがあると、トリガーされたときに正面のブロックの方向を変える。ほかのアイテムがはいっているときはそちらが優先され、確率も含めサボテンは無視される。

### scriptsAppStore
  + 初期値 : `gnembon/scarpet/contents/programs`
  + 使用できる値 : `string`

  scriptをゲーム内でダウンロードするさいの場所を指定する。コンソールにおける`cd`に同じ。github上の有効なパブリックリポジトリのリンクのみ受け付ける。`none`とした場合無効になる。

### scriptsAutoload
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  `/script`が有効になっている場合、serverがリスタートもしくはワールドが読み込まれたときに自動的に読み込まれるようにする。

### scriptsDebugging
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  スクリプトのデバッグメッセージを表示するようにする。
  
### scriptsOptimization
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  スクリプトを最適化する。**一部正常に起動しなくなるスクリプトがあることに注意。**

### sculkSensorRange
  + 初期値 : `8`
  + 使用できる値 : `integer`

  スカルくセンサーの振動を伝える半径を変更する。1から1024の整数値である必要がある。

### shulkerSpawningInEndCities
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  シュルカーがエンドシティーでリスポーンするようにする。
  
### silverFishDropGravel
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  シルバーフィッシュがブロックから抜け出すときに砂利をドロップするようにする。

### simulationDistance
  + 初期値 : `0`
  + 使用できる値 : `integer`

  サーバーのシミュレーション距離をこの値でオーバーライドする。0から32の整数値である必要があり、`0`にすると無効になる。  
  [描画距離の変更](https://github.com/TaichiServer/modDescription/blob/main/carpet.md#viewdistance)

### smoothClientAnimations
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  低いtpsでアニメーションをスムーズにする。さらにシングルプレイではtpsにあわせてプレイヤーの飛行速度が変動するようになる。
  **クライアントのみ**

### spawnChunksSize
  + 初期値 : `11`
  + 使用できる値 : `integer`

  スポーンチャンクの半径を指定する。`0`にするとスポーンチャンクを無効にできる。

### stackableShulkerBoxes
  + 初期値 : `false`
  + 使用できる値 : `string`

  中身のはいっていないシュルカーを地面になげたとき重ねることができる。2から64までの数値または`true` `false`のみを受け付ける。`true`にすると64になる。

### structureBlockIgnored
  + 初期値 : `minecraft:structure_void`
  + 使用できる値 : `string`

  ストラクチャーブロックが無視するブロックのidを指定する。複数指定することはできない。

### structureBlockLimit
  + 初期値 : `48`
  + 使用できる値 : `integer`

  各軸に対するストラクチャーブロックのサイズ制限を変更する。値は48以上でなければならない。  
  **[structureBlockIgnored](https://github.com/TaichiServer/modDescription/blob/main/carpet.md#structureblockignored)をminecraft:airにすることを推奨。**  
  **ストラクチャーブロックが常に読み込まれていなければ正しく動かない**

### structureBlockOutlineDistance
  + 初期値 : `96`
  + 使用できる値 : `integer`

  ストラクチャーブロックのアウトラインを視認できる距離を変更する。値は非負整数でなければならない。
  **クライアントのみ**

### summonNaturalLightning
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  `/summon lightning_bolt`で召喚した稲妻が自然発生した稲妻と同様の効果を与えるようにする。帯電化や炎上など。

### superSecretSetting
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  u306Au3093u3082u308Fu304Bu3089u306Au3044u308821

### thickFungusGrowth
  + 初期値 : `false`
  + 使用できる値 : `false` `random` `all`

  ネザーの菌類を3x3のベースがあるときに太いネザーの菌糸に成長するようにする。　　
 `false`で無効に、`random`で6%の確率で太く、`all`で条件を満たしていればすべて太くなる。 

### tickSyncedWorldBorders
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

ワールドボーダーの見た目の移動が現実時間ではなくtickをもとにするようにする。これによりtpsを変更するとそれに従って見た目上のスピードが変わるようになる。

### tntDoNotUpdate
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  tntが動力源のとなりに置かれたときに自身をupdateしなくする。

### tntPrimerMomentumRemoved
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  着火によるtntの横方向のランダムなモーメントを0にする。

### tntRandomRange
  + 初期値 : `-1.0`
  + 使用できる値 : `double`

  tntの爆発範囲をこの値に設定する。-1.0を除いて正の数でなければならない。  
  **[optimizedTNT](https://github.com/TaichiServer/modDescription/blob/main/carpet.md#optimizedtnt)を有効にする必要がある。**

### updateSuppressionBlock
  + 初期値 : `-1`
  + 使用できる値 : `integer`

  アクティベータレールをバリアブロックの上に置くと、レールがオフになったときに`neighor update stack`が埋められる。この値は、スタックに残すべき更新の量。

### viewDistance
  + 初期値 : `0`
  + 使用できる値 : `integer`

  サーバーの描画距離をこの値でオーバーライドする。0から32の整数値である必要があり、`0`にすると無効になる。  
  [シミュレーション距離の変更](https://github.com/TaichiServer/modDescription/blob/main/carpet.md#simulationdistance)

### xpFromExplosions
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  xpをドロップするブロックはどんな爆発からでもxpをドロップするようにする。

### xpNoCooldown
  + 初期値 : `false`
  + 使用できる値 : `true` `false`

  xpの吸収のクールダウンを消すことができる。











  


