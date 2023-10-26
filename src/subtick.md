<!--
version : v1.0.0
-->
# SubTick
minecraft : `1.20.1`<br>
extra : `1.4.115`

**carpetのaddonであるため、carpetが前提modとなる。**

このドキュメント内では`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はこのリポジトリ内で作成されているcarpetおよびそのaddonのリストである。

|mod|download|document|docs-JP|
|:---:|:---|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|[TIS](./carpet-TIS-addition.html)|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|[extra](./carpet-extra.html)|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](./gugle-carpet-addition.html)|
|Carpet-Fixes|[modrinth](https://modrinth.com/mod/carpet-fixes)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-fixes)*<br>[github](https://github.com/fxmorin/carpet-fixes)|[docs](https://github.com/fxmorin/carpet-fixes/wiki/Available-Settings)|CF|
|intricarpet|[modrinth](https://modrinth.com/mod/intricarpet)<br>[github](https://github.com/lntricate1/intricarpet)|[docs](https://github.com/lntricate1/intricarpet#features)|[intri](./Intricarpet.html)|
|subtick|[modrinth](https://modrinth.com/mod/subtick)<br>[github](https://github.com/chiraagChakravarthy/SubTick)|[docs](https://github.com/chiraagChakravarthy/SubTick#commands)|here|

\* そのサイトでは今後更新がされない

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
### tick
carpetの`/tick`の`freeze`もしくは`step`に対してどこで止めるか、どれだけ進めるかのより深い位置指定が可能になる。それぞれに対して`[phase]`等で指定することでその位置を指定できる。`phase`および`range`のデフォルトはそれぞれのruleで指定されたものを使用する。
+ freeze
  + phase<br>
    `/tick freeze [phase]`でそのフェーズの直前でfreezeもしくはunfreezeする。
+ step
  + phase
    `/tick step [count] [phase]`でそのフェーズの直前までstepさせる。`count`を`0`とすることでphase内でstepさせることができる。
    
tick step [count=1] [phase=subtickDefaultPhase]: Steps count ticks, ending right before phase. Supports tick step 0 [phase] to step to a later phase in the same tick.
phaseStep [count=1]: Steps the count phases forward, stepping to the next tick if necessary.
phaseStep [phase]: Steps to phase, within the current tick.
phaseStep [phase] force: Steps to the next phase stepping to the next tick if necessary.
queueStep <queue> [count=1] [range=subtickDefaultRange]: Steps through count elements in queue in range range, within the current tick. Set range to -1 for unlimited range.
queueStep <queue> [count=1] [range=subtickDefaultRange] force: Steps through count elements in queue in range range, stepping to the next tick if necessary. Set range to -1 for unlimited range.

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