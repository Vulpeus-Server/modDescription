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
+ info

## general
  ### carpet
  #### command: `/carpet`
  現在変更されているcarpetの設定、導入されているcarpetのバージョン、カテゴリーを表示する。
  #### command: `/carpet list [category]`
  `[category]`に紐づけられたruleを表示する。
  
	
## rule
`/carpet [rule] <value>`によって変更することができる。opレベル4以上で使用可能。
  ### allowSpawningOfflinePlayers
  オフラインのプレイヤーを召喚できるかを設定できる。
  オフラインのプレイヤーとは、`/player [mcid] spawn`によるものではなく、
