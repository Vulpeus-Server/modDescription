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
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|here|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](./gugle-carpet-addition.html)|



## 目次
<details>
<summary>rules</summary>

+ [accurateBlockPlacement](#accurateblockplacement)
+ [autoCraftingDropper](#autocraftingdropper)
+ [betterBonemeal](#betterbonemeal)
+ [blazeMeal](#blazemeal)
+ [blockStateSyncing](#blockstatesyncing)
+ [chickenShearing](#chickenshearing)
+ [clericsFarmWarts](#clericsfarmwarts)
+ [commandPing](#commandping)
+ [comparatorBetterItemFrames](#comparatorbetteritemframes)
+ [commparatorReadsClock](#comparatorreadsclock)
+ [creeperSpawningInJungleTemplates](#creeperspawninginjungletemples)
+ [disablePlayerCollision](#disableplayercollision)
+ [dispenserPlacesBlocks](#dispenserplacesblocks)
+ [dispensersCarvePumpkins](#dispenserscarvepumpkins)
+ [dispensersFeedAnimals](#dispensersfeedanimals)
+ [dispensersFillMinecarts](#dispensersfillminecarts)
+ [dispensersMilkAnimals](#dispensersmilkanimals)
+ [dispensersPlaceBoatsOnIce](#dispensersplaceboatsonice)
+ [dispensersPotPlants](#dispenserspotplants)
+ [dispensersStripBlocks](#dispensersstripblocks)
+ [dispensersTillSoil](#dispenserstillsoil)
+ [dispensersToggleThings](#dispenserstogglethings)
+ [dispensersUseCauldrons](#dispensersusecauldrons)
+ [doubleRetraction](#doubleretraction)
+ [dragonEggBedrockBreaking](#dragoneggbedrockbreaking)
+ [emptyShulkerBoxStackAlways](#emptyshulkerboxstackalways)
+ [enderPearlChunkLoading](#enderpearlchunkloading)
+ [fallingBlockDispensers](#fallingblockdispensers)
+ [flowerPotChunkLoading](#flowerpotchunkloading)
+ [hopperMinecartItemTransfer](#hopperminecartitemtransfer)
+ [maxSpongeRange](#maxspongerange)
+ [maxSpongeSuck](#maxspongesuck)
+ [mobInFireConvertsSandToSoulsand](#mobinfireconvertssandtosoulsand)
+ [pistonRedirectsRedstone](#pistonredirectsredstone)
+ [reloadSuffocationFix](#reloadsuffocationfix)
+ [renewableEndstone](#renewableendstone)
+ [renewableIce](#renewableice)
+ [renewableNetherrack](#renewablenetherrack)
+ [renewableSand](#renewablesand)
+ [renewableWitherSkeletons](#renewablewitherskeletons)
+ [repeaterPriorityFix](#repeaterpriorityfix)
+ [scaffoldingDistance](#scaffoldingdistance)
+ [spiderJockeysDropGapples](#spiderjockeysdropgapples)
+ [straySpawningInIgloos](#strayspawninginigloos)
+ [variableWoodDelays](#variablewooddelays)
+ [xpPerSculkCatalyst](#xppersculkcatalyst)
+ [y0DragonEggBedrockBreaking](#y0dragoneggbedrockbreaking)
</details>
<details>
<summary>command</summary>

+ [ping](#ping)
</details>

## rules
全てのルールは`/carpet [rule] [value]`によって変更することができる。
### accurateBlockPlacement
クライアントが特殊なブロックの置き方を可能にするようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### autoCraftingDropper
ドロッパーが作業台を向いていて有効な3x3のクラフトできるレシピを中に含んでいる場合、クラフトされてアイテムをその場にドロップさせる。コンパレータの出力をスロットの占有率で上書きする。また、ホッパー、ドロッパー、ディスペンサーはクラフト可能なドロッパーに対して1スロットにつき1アイテムのみを入れるようになる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### betterBonemeal
骨粉はサトウキビ、サボテン、睡蓮の葉に対しても成長を促進させることができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### blazeMeal
ブレイズパウダーはネザーウォートの繁殖を促すことができるようにする。ディスペンサーもしくは右クリックで有効。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### blockStateSyncing
F3デバッグモードがいくつかのブロックでアップデートを起こさないバグを修正する。ネットワークのトラフィックを増加させる可能性がある。

このバグはmineraft 1.20.2にてバニラで修正済み。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
+ 影響を与えるブロック
	+ サボテン
	+ サトウキビ
	+ 苗木
### chickenShearing
鶏は手またはディスペンサーでハサミを用いて羽をドロップできるようにする。ただしハサミを使うとき鶏はダメージを受ける。子供の鶏はハサミを使うことができない。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### clericsFarmWarts
聖職者はネザーウォーとを植えることできるようにする。これにより聖職者がネザーウォートを取得でき、ソウルサンドをパスファインディングできるようになる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### commandPing
`/ping`を扱えるプレイヤーを設定する。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
+ 関連項目
	+ [ping](#ping)
### comparatorBetterItemFrames
コンパレータは背面に置かれた床もしくは屋根に設置された額縁を読み取れるようにする。
|value|挙動|
|---|---|
|vanilla|バニラ同様の動作|
|behind|背面にある額縁を読み取る|
|lenient|背面もしくはフルブロックを挟んだ背面にある額縁を読み取る|
|extended|背面にあるフルブロックの上にある額縁を読み込む。|
+ 初期値 : `vanilla`
+ 使用できる値 : `vanilla` `behind` `lenient` `extended`
### comparatorReadsClock
コンパレータが額縁にはいっている時計を読むようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### creeperSpawningInJungleTemples
クリーパーはジャングルの寺院**のみ**でスポーンするようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
+ 関連項目
	+ [straySpawningInIgloos](#strayspawninginigloos)
### disablePlayerCollision
プレイヤーの当たり判定をなくす。プレイヤーの当たり判定を利用する回路は壊れるので注意。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispenserPlacesBlocks
ディスペンサーは正面がairである場合ブロックをおけるようになる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersCarvePumpkins
ディスペンサーはハサミ抽選されて正面にかぼちゃがあるときそのかぼちゃをくりぬくことができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersFeedAnimals
ディスペンサーは正面のブロック内に繁殖可能なエンティティがいて繁殖可能なアイテムが抽選された場合、そのアイテムを消費してエンティティを繁殖もしくは増殖できるようにする。茶色のキノコに特定の花を与えて特異なエフェクトを与えることもできる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersFillMinecarts
ディスペンサーは正面のブロックの内部にトロッコがあってカートコンポーネントが抽選された場合、トロッコにカートコンポーネントを乗せることができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersMilkAnimals
ディスペンサーは正面のブロックの内部に牛、ムーシュルーム、ヤギがいて空のバケツが抽選されたとき、牛乳いりバケツにするようにする。ボウルを使うことでシチューにすることもできるようになる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersPlaceBoatsOnIce
Dispensers can place boats on ice
ディスペンサーは正面のブロックがairでその一つ下のブロックに氷があり、ボートが抽選された場合ボートを設置するようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersPotPlants
ディスペンサーは正面に植木鉢があって適切なアイテムが抽選された場合、植木鉢に植えるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersStripBlocks
ディスペンサーは正面に適切なブロックがあって斧が抽選された場合、表皮を剥いだり酸化をもどしたり、ワックスをはがすことができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersTillSoil
ディスペンサーは正面に耕せるブロックがあって鍬が抽選された場合、地面を耕すことができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersToggleThings
ディスペンサーは正面に適切なブロックがあって棒が抽選された場合、正面にあるブロックをトリガーもしくはトグルさせるようにする。例として、ボタンや音ブロックの`powered`やレッドストーンダストの`power`など。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dispensersUseCauldrons
ディスペンサーは大釜に対してアクションを起こせるようにする。内部の変更はもちろん脱色も有効。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### doubleRetraction
ピストンの同一gt内の処理順による再度エフェクトなしの縮小ができるようにする。[MC-88959](https://bugs.mojang.com/browse/MC-88959)を修正する。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### dragonEggBedrockBreaking
1.12に残るドラゴンの卵がlazy chunk内での落下により岩盤を破壊できるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### emptyShulkerBoxStackAlways
インベントリを含め常に空のシュルカーボックスはスタックできるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### enderPearlChunkLoading
水平方向に移動するエンダーパールはentity tickingの段階でチャンクをロードするようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### fallingBlockDispensers
ディスペンサーとドロッパーは正面にあるブロックをfalling blockに変換するようにする。minecraft 22w13oneblockatatimeと同じ速度を与える。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### flowerPotChunkLoading
ウィザーローズがうえられた植木鉢はチャンクをロードさせるようにする。もしこのルールを`true`にする前に植えられた植木鉢があった場合、それらはチャンクをロードさせない。また、このルールが`false`になったときはチャンクのロードが失われず、`/forceload`コマンドによって人力でアンロードすることができる。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### hopperMinecartItemTransfer
ホッパートロッコがアイテムを下のコンテナに移すことができるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### maxSpongeRange
最大のスポンジのオフセットサイズを設定する。
+ 初期値 : `7`
+ 使用できる値 : `integer`
### maxSpongeSuck
最大のスポンジで除去できる水の半径を設定する。**単位はpx**
+ 初期値 : `64`
+ 使用できる値 : `integer`
### mobInFireConvertsSandToSoulsand
もしエンティティが火のついた砂の上で死んだ場合その砂がソウルサンドになるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### pistonRedirectsRedstone
BEのようにピストンと粘着ピストンがレッドストーンダストを曲げるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### reloadSuffocationFix
エンティティがリロードしたときにブロックにめり込むバグを修正するようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### renewableEndstone
ディスペンサーによるドラゴンブレスは丸石をエンドストーンに変換するようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### renewableIce
金床が複数の氷の上におちてきたときより密度の高い氷に変換するようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### renewableNetherrack
ディスペンサーによる火は丸石をネザーラックに変換するようにする。Credits: Skyrising
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### renewableSand
落下する金床が丸石に当たったとき砂をドロップする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### renewableWitherSkeletons
スケルトンが雷に当たった場合ウィザースケルトンに変換されるようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### repeaterPriorityFix
リピーターのセットアップによって短いパルスが失われることがないようにする。[MC-54711](https://bugs.mojang.com/browse/MC-54711)を修正する。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### scaffoldingDistance
最大の足場の距離を設定する。
+ 初期値 : `7`
+ 使用できる値 : `0 ~ 7`
### spiderJockeysDropGapples
スパイダージョッキーは指定されたパーセンテージでエンチャントされた金リンゴを落とすようにする。
+ 初期値 : `0`
+ 使用できる値 : `0 ~ 100`
### straySpawningInIgloos
ストレイはイグルーの内部で**のみ**スポーンするようにする。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
+ 関連項目
	+ [creeperSpawningInJungleTemples](#creeperspawninginjungletemples)
### variableWoodDelays
木製のボタンと感圧版は固有の時間長のロングパルスを発生させる。感圧版は`powered=true`になってからこのgt経過したときに上に乗っているかをチェックし、なにものっていなければ`powered=false`にする。
|variant|button delay(gt)|pressure_plate delay(gt)|
|:---|:---|:---|
|birch|1|1|
|acacia|5|4|
|jungle|15|10|
|oak<br>mangrove<br>cherry<br>bamboo<br>crimson<br>warped|30|20|
|spruce|45|30|
|darkoak|60|40|
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
### xpPerSculkCatalyst
スカルくカタリストが破壊されたときに出されるxpの量を設定する。
+ 初期値 : `5`
+ 使用できる値 : `0 ~`
### y0DragonEggBedrockBreaking
y0もしくはy-64の岩盤をドラゴンの卵で破壊できるようにする。[dragonEggBedrockBreaking](#dragoneggbedrockbreaking)を`true`にする必要がある。
+ 初期値 : `false`
+ 使用できる値 : `true` `false`
+ 関連項目
	+ [dragonEggBedrockBreaking](#dragoneggbedrockbreaking)

## command
### ping
`/ping`でサーバーにpingを送信する。現在のpingが表示される。
+ 関連項目
	+ [commandPing](#commandping)