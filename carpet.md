# carpet

このドキュメント内では
`[]`を設定必須の値、`<>`を設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものは斜線で示す。

[carpet公式ドキュメント](https://github.com/gnembon/fabric-carpet/wiki/Current-Available-Settings)

## 目次
+ general
+ rule
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
+ counter

## general
### carpet
#### `/carpet`
現在変更されているcarpetの設定、導入されているcarpetのバージョン、カテゴリーを表示する。
#### `/carpet list <category>`
利用できるcarpet ruleを**すべて**表示する。`<category>`を指定した場合、紐づけられたruleを表示する。
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
  以下は使用できるコマンドのリスト
  | corlor | command                                      |
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

  `cactus(サボテン)`をメインハンドに持っている時、方向をもつブロックの一部(たとえばホッパーやオブザーバーなど)を右クリックするとその方向をupdateなしで回転もしくは反転できるようにする。

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







