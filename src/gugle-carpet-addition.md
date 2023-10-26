<!--
version : v1.0.1
-->
# gugle-carpet-addition

minecraft : `1.20.1`<br>
GCA : `2.7.0`

**carpetのaddonであるため、carpetが前提modとなる。**

このドキュメント内では`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はこのリポジトリ内で作成されているcarpetおよびそのaddonのリストである。

|mod|download|document|docs-JP|
|:---:|:---|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|[TIS](./carpet-TIS-addition.html)|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|[extra](./carpet-extra.html)|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|here|
|Carpet-Fixes|[modrinth](https://modrinth.com/mod/carpet-fixes)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-fixes)*<br>[github](https://github.com/fxmorin/carpet-fixes)|[docs](https://github.com/fxmorin/carpet-fixes/wiki/Available-Settings)|CF|
|intricarpet|[modrinth](https://modrinth.com/mod/intricarpet)<br>[github](https://github.com/lntricate1/intricarpet)|[docs](https://github.com/lntricate1/intricarpet#features)|[intri](./Intricarpet.html)|
|subtick|[modrinth](https://modrinth.com/mod/subtick)<br>[github](https://github.com/chiraagChakravarthy/SubTick)|[docs](https://github.com/chiraagChakravarthy/SubTick#commands)|ST|

\* そのサイトでは今後更新がされない

## 目次
<details>
<summary>rules</summary>

+ [betterFanceGatePlacement](#betterfancegateplacement)
+ [betterQuickCrafting](#betterquickcrafting)
+ [betterSignInteraction](#bettersigninteraction)
+ [betterWoodStrip](#betterwoodstrip)
+ [fakePlayerAutoFish](#fakeplayerautofish)
+ [fakePlayerAutoReplaceTool](#fakeplayerautoreplacetool)
+ [fakePlayerAutoReplenishment](#fakeplayerautoreplenishment)
+ [fakePlayerReloadAction](#fakeplayerreloadaction)
+ [fakePlayerResident](#fakeplayerresident)
+ [openFakePlayerEnderChest](#openfakeplayerenderchest)
+ [openFakePlayerInventory](#openfakeplayerinventory)
</details>
<details>
<summary>update-logs</summary>

+ [latest](#latest)<br>
  version : `v1.0.1`<br>
  minecraft : `1.20.1`<br>
  GCA : `2.7.0`
+ [previous](#previous)
</details>

## rules
全てのルールは`/carpet [rule] [value]`によって変更することができる。
### betterFanceGatePlacement
フェンスゲートを置くときに見ているフェンスゲートとおなじstateになるように設置するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### betterQuickCrafting
クイッククラフティングをするときインベントリにそのアイテムを残すようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### betterSignInteraction
看板についているブロックを右クリックするとインタラクトすることができるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### betterWoodStrip
`Strip`と名の付く斧のみが原木もしくは木の表皮を剥ぐことができるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### fakePlayerAutoFish
botが釣りでなにかを引き当てたときに自動で釣り上げ、もう一度糸を垂らすようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### fakePlayerAutoReplaceTool
botの使用しているツールがこわれかけているときに、同種のtoolに持ち変えるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### fakePlayerAutoReplenishment
botがtweakerooの`tweakHandRestock`と同様の操作をできるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### fakePlayerReloadAction
botのアクションが再ログイン時にもう一度実行される。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### fakePlayerResident
botがサーバー再起動によっていなくなった時、もう一度同じ座標にスポーンさせる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### openFakePlayerEnderChest
botを右クリックすることでそのプレイヤーのエンダーチェストをGUIで表示・操作できるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
    + [openFakePlayerInventory](#openfakeplayerinventory)
### openFakePlayerInventory
botを右クリックすることでそのプレイヤーのインベントリをGUIで表示・操作できるようにする。すなわちcarpetの`/player`などを介して一つずつ操作する必要をなくすことができる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [player](./carpet.html#player)
    + [openFakePlayerEnderChest](#openfakeplayerenderchest)

## update-logs
### latest
+ version : `v1.0.1`
+ minecraft : `1.20.1`
+ GCA : `2.7.0`
+ 変更点
  + Carpet FixesおよびIntricarpetの参考の追加
+ 更新日<br>
  `23/10/26 UTC+9`
### previous
<details>
<summary>previous</summary>
<details>
<summary><code>v1.0.0</code></summary>

+ minecraft : `1.20.1`
+ GCA : `2.7.0`
+ 変更点
  + 誤字の訂正
+ 更新日<br>
  `2023/10/16 UTC+9`
</details>
<details>
<summary><code>v0.0.0</code></summary>

+ minecraft : `1.20.1`
+ GCA : `2.7.0`
+ 変更点
  + ドキュメントの作成
+ 更新日<br>
  `2023/10/16 UTC+9`
</details>
</details>