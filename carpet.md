# carpet

このドキュメント内では
`[]`を設定必須の値、`<>`を設定しなかった場合デフォルトの値が入力される値とする。
また、特に記述がない

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
	
## rule
`/carpet [rule] <value>`によって変更することができる。opレベル4以上で使用可能。
  ### allowSpawningOfflinePlayers
  オフラインのプレイヤーを召喚できるかを設定できる。
  オフラインのプレイヤーとは、`/player [mcid] spawn`によるものではなく、
