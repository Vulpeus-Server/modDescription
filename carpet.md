# carpet

このドキュメント内では
`[]`を設定必須の値、`<>`を設定しなかった場合デフォルトの値が入力される値とする。

[carpet公式ドキュメント](https://github.com/gnembon/fabric-carpet/wiki/Current-Available-Settings)

## 目次
+ general
+ rule
+ tick
+ player
+ profile
+ log

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
### allowSpawningOfflinePlayers
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




