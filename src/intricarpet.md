<!--
version : v1.0.0
-->
# Intricarpet
minecraft : `1.20.1`<br>
extra : `1.4.115`

**carpetのaddonであるため、carpetが前提modとなる。**

このドキュメント内では`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はこのリポジトリ内で作成されているcarpetおよびそのaddonのリストである。

|mod|download|document|docs-JP|
|:---:|:---|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://tisunion.github.io/Carpet-TIS-Addition/docs)|[TIS](./carpet-TIS-addition.html)|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|[extra](./carpet-extra.html)|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](./gugle-carpet-addition.html)|
|intricarpet|[modrinth](https://modrinth.com/mod/intricarpet)<br>[github](https://github.com/lntricate1/intricarpet)|[docs](https://github.com/lntricate1/intricarpet#features)|here|

## 目次
<details>
<summary>rules</summary>

+ [commandInteraction](#commandinteraction)
</details>
<details>
<summary>command</summary>

+ [interaction](#interaction)
+ [log](#log)
</details>
<details>
<summary>update-logs</summary>

+ [latest](#latest)<br>
  version : `v1.0.0`<br>
  minecraft : `1.20.1`<br>
  extra : `v2.0.1`
+ [previous](#previous)
</details>

## rules
全てのルールは`/carpet [rule] [value]`によって変更することができる。
### commandInteraction
`/interaction`を使用できるプレイヤーを指定する。
+ 初期値 : `ops`
+ 使用できる値 : `true` `false` `ops`
+ 関連項目
    + [interaction](#interaction)

## command
### interaction
`/interaction <interaction> <true | false>`でそれぞれのクライアントからサーバーへの各interactionの送信の可否を切り替えることができる。`<interaction>`を指定しなかった場合、現在の設定を表示する。クライアント事に決めることができる。また、`<true | false>`を指定しなかった場合そのinteractionの設定を表示する。
<details>
<summary>interaction</summary>

+ `blocks`<br>
  トリップワイヤーや感圧版の検知、耕地の踏み荒らしなどのブロックの変更をするものを変更する。
+ `chunkloading`<br>
  テレポートチケットを含むすべてのプレイヤーのチャンクの読み込みを変更する。
+ `entities`<br>
  他のプレイヤーを含むすべてのエンティティが自身に対して無視するように変更する。
+ `mobSpawning`<br>
  スポーンエッグを除くそのプレイヤーからのmobのスポーンを変更する。ただしmobcapsには影響を与えない。
+ `randomTicks`<br>
  そのプレイヤーからのrandom tickを変更する。
+ `updates`<br>
  全てのプレイヤーがワールドに与えるべきupdateを変更する。
</details>

+ 関連項目
	+ [commandInteraction](#commandinteraction)
  + carpet / [creativeNoClip](./carpet.html#crativenoclip)
  + carpet / [creativePlayersLoadChunks](./carpet.html#creativeplayerloadchunks)
  + TIS / [totallyNoBlockUpdate](./carpet-TIS-addition.html#totallynoblockupdate)

### log
carpetの`/log explosion`に`compact`を追加する。複数のtntが同じtickで爆発するとき、その爆発する座標でグルーピングするようにする。
+ 関連項目
  + carpet / [log](./carpet.html#log)

## update-logs
### latest
+ version : `v1.0.0`
+ minecraft : `1.20.1`
+ extra : `v2.0.1`
+ 変更点
  + ドキュメントの作成
+ 更新日<br>
  `23/10/26 UTC+9`
### previous
<details>
<summary>previous</summary>
</details>