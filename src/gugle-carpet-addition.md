# gugle-carpet-addition

version : GCA 2.7.0

**carpetのaddonであるため、carpetが前提modとなる。**

このドキュメント内では`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はcarpetおよびそのaddonで日本語ドキュメントが存在もしくは作られる予定のリストである。

|mod|download|document|docs-JP|
|:---:|:---:|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|[TIS](./carpet-TIS-addition.html)|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|[extra](./carpet-extra.html)|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|here|



## 目次
<details>
<summary>rules</summary>

+ [openFakePlayerInventory](#openfakeplayerinventory)
+ [openFakePlayerEnderChest](#openfakeplayerenderchest)
+ [fakePlayerResident](#fakeplayerresident)
+ [fakePlayerAutoReplenishment](#fakeplayerautoreplenishment)
+ [fakePlayerAutoFish](#fakeplayerautofish)
+ [fakePlayerAutoReplaceTool](#fakeplayerautoreplacetool)
</details>

## rules
全てのルールは`/carpet [rule] [value]`によって変更することができる。
### openFakePlayerInventory
fake playerを右クリックすることでそのプレイヤーのインベントリをGUIで表示・操作できるようにする。すなわちcarpetの`/player`などを介して一つずつ操作する必要をなくすことができる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
    + [openFakePlayerEnderChest](#openfakeplayerenderchest)

### openFakePlayerEnderChest
fake playerを右クリックすることでそのプレイヤーのエンダーチェストをGUIで表示・操作できるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
    + [openFakePlayerInventory](#openfakeplayerinventory)

### fakePlayerResident
fake playerがサーバー再起動によっていなくなった時、次回起動時に自動でplayerを配置し、そのplayerが実行しているactionを再実行させる。ただし正しいtickで実行されるのではなく、もう一度コマンドをたたいているだけなので信用はできない。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)

### fakePlayerAutoReplenishment
fake playerがtweakerooの`tweakHandRestock`と同様の操作をできるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)

### fakePlayerAutoFish
fake playerが釣りでなにかを引き当てたときに自動で釣り上げ、もう一度糸を垂らすようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)

### fakePlayerAutoReplaceTool
fake playerの使用しているツールがこわれたときに、同種のtoolに持ち変えるようにする。ただし耐久が少し残る等はない。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)