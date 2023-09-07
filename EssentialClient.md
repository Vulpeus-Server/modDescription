# Essential Client
Version 1.3.6

- [Modrinth](https://modrinth.com/mod/essentialclient)
- [GitHub](https://github.com/senseiwells/EssentialClient)

## Features

### client script

クライアント用のスクリプトを実行することができる。スクリプトには[Arucas](https://github.com/senseiwells/Arucas)という言語を使う。詳細なドキュメントは[EssentialClient/docs/Full.md](https://github.com/senseiwells/EssentialClient/blob/main/docs/Full.md)から確認できる。またClient Script Optionsメニューからいくつかのサンプルスクリプトをダウンロードできる。

### chunk debug

ロードされているチャンクを監視できる機能。ミニマップとして表示することもできる。

### carpet client

carpetのゲームルールをGUIで変更できる。ただしサーバーにcarpetがインストールされておりかつ適切な権限を持っている必要がある。変更できるゲームルールは[Carpet Rules Database](https://carpet-rules.crec.dev/)を参照している。

### gamerule screen

MinecraftのゲームルールをGUIで変更できる。ただしサーバー環境においてはEssentialAddonsがインストールされている必要がある、

## Options

### Essential Client Options

#### afkLogout

設定したtick数無操作の状態が続くと自動的に切断する。

- 初期値: `0`
- 有効な値: `200`以上の整数値

#### announceAFK

指定したtick数プレイヤーの位置が変わらなかった場合に[announceAFKMessage](#announceafkmessage)で指定したメッセージをチャットに送信する。

- 初期値: `0`
- 有効な値: `Integer`

#### announceAFKMessage

[announceAFK](#announceafk)で送信するメッセージ。

- 初期値: `I am now AFK`
- 有効な値: `String`

#### announceBackMessage

[announceAFK](#announceafk)によるAFK状態が解除されたときに送信するメッセージ。

- 初期値: ` `
- 有効な値: `String`

#### autoWalk

指定したtick数前進を入力し続けると自動で前進するようになる。再び前進を入力するか後退を入力すると停止できる。

- 初期値: `0`
- 有効な値: `Integer`

#### betterAccurateBlockPlacement

tweakerooのaccurate block placement機能と同じ。

#### carpetAlwaysSetDefault

carpetのゲームルールを変更した際にそれをデフォルトの設定値にする。同modのCarpet Server Optionsで変更した場合にも有効。

- 初期値: `false`
- 有効な値: `Boolean`

#### chunkDebugMinimapBackground

chunk debugミニマップで背景を描画する。

- 初期値: `true`
- 有効な値: `Boolean`

#### clientDebugShowUnloadedChunks

ChunkDebugでアンロードされているチャンクを表示する。

- 初期値: `false`
- 有効な値: `Boolean`

#### clientScriptAnnouncements

[client script](#client-script)が開始/終了した際にチャットを送信する。

- 初期値: `true`
- 有効な値: `Boolean`

#### clientScriptFont

[client script](#client-script)のエラーメッセージのフォントを変更する。

- 初期値: `Minecraft`
- 有効な値: `Minecraft` `Jetbrains`

#### clientScriptRepos

scriptをダウンロードするレポジトリを指定する。レポジトリは複数指定できる。

- 初期値: `https://api.github.com/repos/senseiwells/clientscript/contents/scripts`

#### commandAlternateDimension

自分がいる座標の別ディメンション(オーバーワールドかネザー)での値を取得するコマンド`/alternatedimension`を有効にする。出力された座標をクリックするか、`/alternatedimension teleport`を実行することでそのディメンションの座標にテレポートする。

- 初期値: `false`
- 有効な値: `Boolean`

#### commandClientNick

クライアント上でのプレイヤーのニックネームを変更する`/clientnick`コマンドを有効にする。ニックネームには任意の文字列を指定できる。(ただしMinecraft装飾コードの`§`は`&`に置き換えて使用する)

- 初期値: `false`
- 有効な値: `Boolean`

#### commandPlayerClient

carpetの`/player`コマンドを保存し実行する`/playerclient`コマンドを有効にする。

- 初期値: `false`
- 有効な値: `Boolean`

<details>
<summary>コマンドの詳細</summary>

#### `/playerclient`コマンドの使い方

[wiki](https://github.com/senseiwells/EssentialClient/wiki/CommandPlayerClient)

- `/playerclient add...`
指定したプレイヤーをconfigに保存する。スポーンする座標、顔の向き、スポーンするディメンション、ゲームモードも合わせて指定して保存できる。

```
/playerclient add [name] spawn at [x] [y] [z] facing [yaw] [pitch] in [dimension] in [gamemode]

/playerclient add [name] spawn here in [gamemode]
```

- `/playerclient remove...`
指定したプレイヤーをconfigから削除する。

```
/playerclient remove [name]
```

- `/playerclient spawn...`
configに保存されたプレイヤーを指定してスポーンさせる。保存されている座標からのオフセットを指定してその座標にスポーンさせることもできる。

```
/playerclient spawn [name]
/playerclient spawn [name] offset [x] [y] [z]
```

保存した情報は`config/EssentialClient/PlayerClient.json`に保存されている。
例
```json
{
  "steve": {
    "x": 0.5,
    "y": 73.0,
    "z": 0.5,
    "yaw": 0.0,
    "pitch": 0.0,
    "dimension": "overworld",
    "gamemode": "creative"
  }
}
```
</details>

#### commandPlayerList

`/playerclient`コマンドで保存した複数のプレイヤーを一度にスポーンさせる`/playerlist`コマンドを有効にする。

- 初期値: `false`
- 有効な値: `Boolean`

<details>
<summary>コマンドの詳細</summary>

#### `/playerlist`コマンドの使い方

[wiki](https://github.com/senseiwells/EssentialClient/wiki/CommandPlayerList)

- `/playerlist createlist...`
リストを新規作成する。

```
/playerlist createlist [list_name]
```

- `/playerlist deletelist...`
リストを削除する。

```
/playerlist deletelist [list_name]
```

- `/playerlist addplayer...`
プレイヤーをリストに加える。指定するプレイヤーは先に`/playerclient`コマンドで保存しておく必要がある。

```
/playerlist addplayer [list_name] [player_name]
```

- `/playerlist spawnlist...`
リストに登録されているプレイヤー全員をスポーンさせる。

```
/playerlist spawnlist [list_name]
```

保存した情報は`config/EssentialClient/PlayerList.json`に保存されている。
例
```json
{
  "foo": [
    "alex",
    "steve"
  ]
}
```
</details>

#### commandRegion

プレイヤーがいる座標あるいは指定した座標のregionを取得するコマンド`/region`を有効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### commandSuggesterIgnoresSpaces

コマンドの入力時に余分なスペースを入れても補完されるようにする。

- 初期値: `false`
- 有効な値: `Boolean`

#### craftingHax

Ctrlキーを押しながらレシピをクリックすることでアイテムをクラフトしてドロップする。Shiftキーも同時に押すことでスタックごとクラフトしてドロップする。

- 初期値: `false`
- 有効な値: `Boolean`

#### customClientCape

指定したマントを着用する。自分のクライアント側でのみ描画される。
マントのデザインは[マント - Minecraft Wiki](https://minecraft.fandom.com/ja/wiki/%E3%83%9E%E3%83%B3%E3%83%88#%E3%83%87%E3%82%B6%E3%82%A4%E3%83%B3)で確認できる。

- 初期値: `None`
- 有効な値: `None` `Old Mojang` `Mojang` `Mojang Studios` `Minecon 2011` `Minecon 2012`
`Minecon 2013` `Minecon 2015` `Minecon 2016` `Bacon` `Millionth` `DannyB` `Julian`
`Cheapsh0t` `MrMessiah` `Prismarine` `Birthday` `Translator` `Scrolls` `Cobalt` `Mojira`
`Turtle` `Migrator` `Christmas 2010` `New Year 2011`

#### disableArmourRendering

指定したエンティティのアーマーの描画を無効にする。

- 初期値: `None`
- 有効な値: `None` `You` `Players` `Entities`

#### disableBobViewWhenHurt

自分がダメージを受けた際のカメラの揺れを無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableBossBar

ボスバーの描画を無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableHotbarScrolling

ホットバーのスクロールを無効にする。ホットキーを使うことを学ぼう😀

- 初期値: `false`
- 有効な値: `Boolean`

#### disableJoinLeaveMessage

参加/退出のメッセージを非表示にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableMapRendering

地図を入れた額縁の描画を無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableNameTags

プレイヤーのネームタグを非表示にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableNarrator

Ctrl + Bを入力した際のナレーター切り替えを無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableNightVisionFlash

暗視効果が切れる前の画面の点滅を無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableOpMessages

システムメッセージを非表示にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableRecipeNotifications

レシピを解放した際のトースト通知を非表示にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableScreenshotMessage

スクリーンショットを撮影した際のメッセージを無効にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### disableTutorialNotifications

チュートリアルのトースト通知を非表示にする。

- 初期値: `false`
- 有効な値: `Boolean`

#### displayRuleType

ゲームルールの表示順を切り替える。

- 初期値: `Alphabetical`
- 有効な値: `Alphabetical` `Rule Type` `Categories`

#### displayTimePlayed

ポーズメニューを開いた際に現在のプレイ時間を表示する。これによりどれだけの時間を~~無駄にしたか~~生産的に過ごしたかを知ることができる。

- 初期値: `false`
- 有効な値: `Boolean`

#### essentialClientButton

ポーズメニューとメインメニューでEssential Client Buttonを表示する。

- 初期値: `true`
- 有効な値: `Boolean`

#### highlightLavaSources

溶岩源をハイライトする。

- 初期値: `false`
- 有効な値: `Boolean`

#### highlightWaterSources

水源をハイライトする。

- 初期値: `false`
- 有効な値: `Boolean`

#### increaseSpectatorScrollSensitivity

スペクテイターモードでより速く移動するためにマウスホイールをスクロールする時の感度を上げる。尚Minecraft標準ではダッシュキーありでの最高速度が87.111 m/sとなっている。 (参考: [スペクテイター - Minecraft Wiki](https://minecraft.fandom.com/ja/wiki/%E3%82%B9%E3%83%9A%E3%82%AF%E3%83%86%E3%82%A4%E3%82%BF%E3%83%BC#%E9%A3%9B%E8%A1%8C))

- 初期値: `0`
- 有効な値: `Integer`

#### increaseSpectatorScrollSpeed

スペクテイターモードでより速く移動するためにスクロールできる限度を上げる。

- 初期値: `false`
- 有効な値: `Boolean`

#### openScreenshotDirectory

スクリーンショットのメッセージリンクをクリックした際にスクリーンショットのディレクトリを開くようにする。

- 初期値: `false`
- 有効な値: `Boolean`

#### overrideCreativeWalkSpeed

クリエイティブモードでの移動速度を変更する。クリエイティブモード限定なのでずるをしようとは考えないように。

- 初期値: `0.0`
- 有効な値: `Double`

#### permanentChatHud

ワールドやサーバーから退出した時も含めて常にチャット履歴が残るようにする。

- 初期値: `false`
- 有効な値: `Boolean`

#### permanentTime

クライアント側の時間を指定した値で固定する。

- 初期値: `-1`
- 有効な値: `-1` `0-23999`

#### quickLockRecipe

レシピをホイールクリックした際に検索欄をそのレシピで固定する。レシピ以外の場所や他のレシピをホイールクリックすることで固定を変更することができる。

- 初期値: `false`
- 有効な値: `Boolean`

#### removeWarnReceivedPassengers

クライアントの"Received passengers for unknown entity"の警告を削除する。

- 初期値: `false`
- 有効な値: `Boolean`

#### soulSpeedFovMultiplier

ソウルスピードによる視野角の倍率を変更する。

- 初期値: `0.0`
- 有効な値: `0.00-1.00`

#### stackableShulkersInPlayerInventories

空のシュルカーボックスのItemsタグを削除することによりインベントリ内でのシュルカーボックスのスタックを有効にする。ただしサーバー側にEssentialAddonsがインストールされておりかつサーバー側で`stackableShulkersInPlayerInventories`が有効になっている必要がある。

- 初期値: `false`
- 有効な値: `Boolean`

#### stackableShulkersWithItems

インベントリ内でのアイテムが入っているシュルカーボックスのスタックを有効にする。ただし[stackableShulkersInPlayerInventories](#stackableshulkersinplayerinventories)が有効になっている必要がある。

#### startSelectedScriptsOnJoin

ワールドに入った際に指定したClientScriptを実行する。

- 初期値: `false`
- 有効な値: `Boolean`

#### survivalInventoryInCreative

クリエイティブモードでサバイバルモードのインベントリを開くことができるようにする。

- 初期値: `false`
- 有効な値: `Boolean`

#### switchToTotem

体力が指定した値を下回った際に不死のトーテムに持ち替える。

- 初期値: `0`
- 有効な値: `Integer`

#### titleTextToTop

MinecraftのバージョンとMojangのテキストの表示をスクリーン上部に変更する。

- 初期値: `false`
- 有効な値: `Boolean`

#### toggleTab

TABを長押し式からトグル式に切り替える。

- 初期値: `false`
- 有効な値: `Boolean`

#### unlockAllRecipesOnJoin

ワールドに入った際に全てのレシピを解放する。

- 初期値: `false`
- 有効な値: `Boolean`

#### waterFovMultiplier

水中での視野角の倍率を変更する。

- 初期値: `0.0`
- 有効な値: `0.00-1.00`
