# carpet TIS addition
version : TIS 1.50.1
<!--
version : v1.0.0
-->
**carpetのaddonであるため、carpetが前提modとなる。**

このドキュメント内では`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はこのリポジトリ内で作成されているcarpetおよびそのaddonのリストである。

|mod|download|document|docs-JP|
|:---:|:---|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|here|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)|[extra](./carpet-extra.html)|
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](./gugle-carpet-addition.html)|
|Carpet-Fixes|[modrinth](https://modrinth.com/mod/carpet-fixes)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-fixes)❌<br>[github](https://github.com/fxmorin/carpet-fixes)||CF|
|intricarpet|[modrinth](https://modrinth.com/mod/intricarpet)<br>[github](https://github.com/lntricate1/intricarpet)||intri|



## 目次
<details>
  <summary>general</summary>

  + [carpet-rule-tweaks](#carpet-rule-tweaks)
  + [carpet-command-tweaks](#carpet-command-tweaks)
</details>

<details>
  <summary>rules</summary>

  + [antiSpamDisabled](#antispamdisabled)
  + [blockEventPacketRange](#blockeventpacketrange)
  + [blockPlacementIgnoreEntity](#blockplacementignoreentity)
  + [chunkTickSpeed](#chunktickspeed)
  + [clientSettingsLostOnRespawnFix](#clientsettingslostonrespawnfix)
  + [commandLifeTime](#commandlifetime)
  + [commandManipulate](#commandmanipulate)
  + [commandRaid](#commandraid)
  + [commandRaycast](#commandraycast)
  + [commandRefresh](#commandrefresh)
  + [commandRemoveEntity](#commandremoveentity)
  + [commandSleep](#commandsleep)
  + [creativeNetherWaterPlacement](#creativenetherwaterplacement)
  + [creativeNoItemCooldown](#creativenoitemcooldown)
  + [creativeOpenContainerForcibly](#creativeopencontainerforcibly)
  + [deobfuscateCrashReportStackTrace](#deobfuscatecrashreportstacktrace)
  + [dispenserNoItemCost](#dispensernoitemcost)
  + [dispensersFireDragonBreath](#dispensersfiredragonbreath)
  + [enchantCommandNoRestriction](#enchantcommandnorestriction)
  + [entityMomentumLoss](#entitymomentumloss)
  + [entityPlacementIgnoreCollision](#entityplacementignorecollision)
  + [entityTrackerDistance](#entitytrackerdistance)
  + [entityTrackerInterval](#entitytrackerinterval)
  + [explosionNoEntityInfluence](#explosionnoentityinfluence)
  + [explosionPacketRange](#explosionpacketrange)
  + [failSoftBlockStateParsing](#failsoftblockstateparsing)
  + [fakePlayerNamePrefix](#fakeplayernameprefix)
  + [fakePlayerNameSuffix](#fakeplayernamesuffix)
  + [fakePlayerRemoteSpawning](#fakeplayerremotespawning)
  + [farmlandTrampledDisabled](#farmlandtrampleddisabled)
  + [fillCommandModeEnhance](#fillcommandmodeenhance)
  + [flattenTriangularDistribution](#flattentriangulardistribution)
  + [fluidDestructionDisabled](#fluiddestructiondisabled)
  + [hopperCountersUnlimitedSpeed](#hoppercountersunlimitedspeed)
  + [hopperNoItemCost](#hoppernoitemcost)
  + [HUDLoggerUpdateInterval](#hudloggerupdateinterval)
  + [instantBlockUpdaterReintroduced](#instantblockupdaterreintroduced)
  + [instantCommandBlock](#instantcommandblock)
  + [itemEntitySkipMovementDisabled](#itementityskipmovementdisabled)
  + [keepMobInLazyChunks](#keepmobinlazychunks)
  + [largeBarrel](#largebarrel)
  + [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)
  + [lightQueueLoggerSamplingDuration](#lightqueueloggersamplingduration)
  + [lightUpdates](#lightupdates)
  + [loggerMovement](#loggermovement)
  + [microTiming](#microtiming)
  + [microTimingDyeMarker](#microtimingdyemarker)
  + [microTimingTarget](#microtimingtarget)
  + [microTimingTickDivision](#microtimingtickdivision)
  + [minecartFullDropBackport](#minecartfulldropbackport)
  + [minecartTakePassengerMinVelocity](#minecarttakepassengerminvelocity)
  + [mobcapsDisplayIgnoreMisc](#mobcapsdisplayignoremisc)
  + [oakBalloonPercent](#oakballoonpercent)
  + [observerNoDetection](#observernodetection)
  + [opPlayerNoCheat](#opplayernocheat)
  + [optimizedFastEntityMovement](#optimizedfastentitymovement)
  + [optimizedHardHitBoxEntityCollision](#optimizedhardhitboxentitycollision)
  + [optimizedTNTHighPriority](#optimizedtnthighpriority)
  + [poiUpdates](#poiupdates)
  + [persistentLoggerSubscription](#persistentloggersubscription)
  + [preciseEntityPlacement](#preciseentityplacement)
  + [railDupingFix](#raildupingfix)
  + [redstoneDustRandomUpdateOrder](#redstonedustrandomupdateorder)
  + [renewableDragonEgg](#renewabledragonegg)
  + [renewableDragonHead](#renewabledragonhead)
  + [renewableElytra](#renewableelytra)
  + [repeaterHalfDelay](#repeaterhalfdelay)
  + [sandDupingFix](#sanddupingfix)
  + [snowMeltMinLightLevel](#snowmeltminlightlevel)
  + [stopCommandDoubleConfirmation](#stopcommanddoubleconfirmation)
  + [structureBlockDoNotPreserveFluid](#structureblockdonotpreservefluid)
  + [synchronizedLightThread](#synchronizedlightthread)
  + [syncServerMsptMetricsData](#syncservermsptmetricsdata)
  + [tileTickLimit](#tileticklimit)
  + [tiscmNetworkProtocol](#tiscmnetworkprotocol)
  + [tntDupingFix](#tntdupingfix)
  + [tntIgnoreRedstoneSignal](#tntignoreredstonesignal)
  + [tntFuseDuration](#tntfuseduration)
  + [tooledTNT](#tooledtnt)
  + [totallyNoBlockUpdate](#totallynoblockupdate)
  + [toughWitherRose](#toughwitherrose)
  + [turtleEggTrampledDisabled](#turtleeggtrampleddisabled)
  + [undeadDontBurnInSunlight](#undeaddontburninsunlight)
  + [updateSuppressionSimulator](#updatesuppressionsimulator)
  + [visualizeProjectileLoggerEnabled](#visualizeprojectileloggerenabled)
  + [voidDamageAmount](#voiddamageamount)
  + [voidDamageIgnorePlayer](#voiddamageignoreplayer)
  + [voidRelatedAltitude](#voidrelatedaltitude)
  + [witherSpawnedSoundDisabled](#witherspawnedsounddisabled)
  + [ported-rules](#ported-rules)
    + [lightEngineMaxBatchSize](#lightenginemaxbatchsize)
    + [yeetUpdateSuppressionCrash](#yeetupdatesuppressioncrash)
</details>

<details>
<summary>command</summary>

  + [info](#info)
  + [lifetime](#lifetime)
  + [log](#log)
  + [manipulate](#manipulate)
  + [player](#player)
  + [raid](#raid)
  + [raycast](#raycast)
  + [reflesh](#reflesh)
  + [removeentity](#commandremoveentity)
  + [scounter](#scounter)
  + [sleep](#sleep)
  + [spawn](#spawn)
  + [tick](#tick)
</details>
<details>
<summary>update-logs</summary>

+ [latest](#latest)<br>
  version : `v1.0.0`<br>
  TIS : `1.50.1`
+ [previous](#previous)
</details>

## general
これらはすべて設定などはなく、導入した時点ですべて適用される。
### carpet-rule-tweaks
+ tntRandomRangeの変更<br>
  carpetの[tntRandomRange](./carpet.html#tntrandomrange)が[lithium](https://modrinth.com/mod/lithium)もしくは[optimizedTNT](./carpet.html#optimizedtnt)なしでも動くようになる。
+ creativeNoClipの強化<br>
  creativeNoClipがtrueのときゲームは以下のリストにあるアクションをするときプレイヤーを無視するようにする。
  + Dispenser block placement<br>
    ディスペンサーがブロックを置く。
  + Xp orb tracking<br>
    Xp orbがプレイヤーを追跡する。
  + Tripwire and pressure plate detecting<br>
    トリップワイヤーもしくは感圧版がプレイヤーを検出する。
  + Entity movement caused by block change, e.g. farmland being broken<br>
    プレイヤーの移動によるブロックの変更。
  + Calculation of collision boxes from entities<br>
    当たり判定の計算。ボートやトロッコの移動や設置など。
### Carpet-Command-Tweaks
+ tick<br>
  fabric-carpet v1.4.18以前の`/tick warp`における最大値をなくす。v1.4.18以降ではcarpetがそれを廃止したため事実上無意味となった。
+ carpet<br>
  `/carpet`を実行したときcarpet-TIS-additionのバージョンを表示する。

## rules
  全てのルールは`/carpet [rule] <value>`によって変更することができる。
### antiSpamDisabled
  サーバーによるプレイヤーのスパムチェックを無効にする。これにはメッセージのクールダウンやアイテムのドロップ量に関する閾値が含まれる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [antiCheatDisabled](./carpet.md#anticheatdisabled)
### blockEventPacketRange
  block updateが正しく起動したときに送信するpacketの範囲を指定する。パケット量超過によるタイムアウトを防止するのに役立つが、このパケットはクライアントの描画の同期に使われるので値を低くしすぎると正しく動作していないように**みえる**可能性がある。
  + 初期値 : `64`
  + 使用できる値 : `double`
  + 関連項目
    + [explosionPacketRange](#explosionpacketrange)
  <div class="md-note">
    これは実際に見えるだけであり、実際には処理される。シングルではシミュレーション距離で上書きされる。
  </div>

### blockPlacementIgnoreEntity
  クリエイティブにおいて、プレイヤーの当たり判定を無視してブロックをおけるようにする。entity全般にたいしてではないことに注意。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [entityPlacementIgnoreCollision](#entityplacementignorecollision)
### chunkTickSpeed
  chunk tickの1チャンク*gtにおける発生量を制御する。`0`にすることで無効にできる。落雷が発生する場所や積雪、水源の氷結、そしてrandom tickが効果を受ける。random tickでは1chunk tickに対して`randomTickSpeed`の数だけ発生する。
  + 初期値 : `1`
  + 使用できる値 : `integer`
### clientSettingsLostOnRespawnFix
  クライアントに保存される設定がプレイヤーのリスポーンもしくはエンドへ入ったときにサーバー側が認識できなくなるバグを修正する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### commandLifeTime
  `/lifetime`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [lifetime](#lifetime)
### commandManipulate
  `/manipulate`を使用できるプレイヤーを指定する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [manipulate](#manipulate)
### commandRaid
  `/raid`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [raid](#raid)
### commandRaycast
  `/raycast`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [raycast](#raycast)
### commandRefresh
  `/refresh`を使用できるプレイヤーを指定する。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [refresh](#refresh)
### commandRemoveEntity
  `/removeentity`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [removeentity](#removeentity)
### commandSleep
  `/sleep`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + [sleep](#sleep)
### creativeNetherWaterPlacement
  クリエイティブのプレイヤーがネザーで水を置けるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### creativeNoItemCooldown
  クリエイティブのプレイヤーのクールダウンをなくすようにする。例えばエンダーパールをなげたあとの20gtのクールダウンなど。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### creativeOpenContainerForcibly
  クリエイティブのプレイヤーがブロックされたコンテナを強制的にあけられるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### deobfuscateCrashReportStackTrace
  クラッシュレポートのstack traceの難読化を解除する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### dispenserNoItemCost
  ディスペンサーとドロッパーがトリガーするとき、内部のアイテムを減らさないでトリガーさせるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [hopperCounter](./carpet.html#hoppercounters)
### dispensersFireDragonBreath
  ディスペンサーがドラゴンブレスをトリガーしたとき、正面のブロックに対してドラゴンブレスを生成させることができるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### enchantCommandNoRestriction
  `/enchant`コマンドはいかなるエンチャントの競合を無視するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### entityMomentumLoss
  ロードした瞬間のエンティティの速度が10m/gtを超えたときに発生する各軸のモーメンタムを10m/gtに抑え込むようにする。
  + 初期値 : `true`
  + 使用できる値 : `true` `false`
### entityPlacementIgnoreCollision
  防具立、ボート、エンドクリスタルを配置するときにブロックと他のentityの当たり判定のチェックを行わないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [blockPlacementIgnoreEntity](#blockplacementignoreentity)
### entityTrackerDistance
  エンティティが同期される最大距離。ただしチャンクに対するチェビシェフ距離である。基本的にこの値はサーバーでのエンティティ描画距離として機能するため、サーバーの描画距離までに制限される。負の数とするとバニラの挙動にすることができる。
  + 初期値 : `-1`
  + 使用できる値 : `integer`
  + 関連項目
    + [entityTrackerInterval](#entitytrackerinterval)
  <details>
  <summary>チェビシェフ距離の定義</summary>

  \\(xz\\)座標平面上にある点\\(P_1(x_1,z_1),P_2(x_2,z_2)\\)において、チェビシェフ距離 \\(d(P_1,P_2)\\)は

  $$d(P_1,P_2):=max(|x_1-x_2|,|z_1-z_2|)$$

  </details>

### entityTrackerInterval
  エンティティの同期の周期を設定する。負の数を指定した場合バニラの挙動にすることができる。
  + 初期値 : `-1`
  + 使用できる値 : `integer`
  + 関連項目
    + [entityTrackerDistance](#entitytrackerdistance)
### explosionNoEntityInfluence
  爆発物は**いかなる**エンティティに対して影響を及ぼさないようにする。これにはダメージのほか、モーメンタム等も含まれる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### explosionPacketRange
  爆発が発生したときに送信されるパケットの範囲を指定する。負の数を指定することでバニラの挙動になる。
  + 初期値 : `-1`
  + 使用できる値 : `integer`
  + 関連項目
    + [blockEventPacketRange](#blockeventpacketrange)
### failSoftBlockStateParsing
  `/setblock`などで正しくない値やタグを持たせた場合、その値やタグを含む部分**のみ**を無視して実行させるようにする。
  たとえばこのルールを`true`にした状態で`/setblock ~ ~ ~ piston[extended=t,facing=up]`を実行すると、`extend`が初期値である`false`の状態で上向きピストンが配置される。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### fakePlayerNamePrefix
  `/player`によって召喚されたbotに前置詞をつける。botの名前に付与されるので、16文字以内かつ英数字と`_`のみしか使用できない。`#none`とするとprefixを無効にできる。
  + 初期値 : `#none`
  + 使用できる値 : `string`
  + 関連項目
    + [fakePlayerNameSuffix](#fakeplayernamesuffix)
### fakePlayerNameSuffix
  `/player`によって召喚されたbotに後置詞をつける。botの名前に付与されるので、16文字以内かつ英数字と`_`のみしか使用できない。`#none`とするとsuffixを無効にできる。
  + 初期値 : `#none`
  + 使用できる値 : `string`
  + 関連項目
    + [fakePlayerNamePrefix](#fakeplayernameprefix)
### fakePlayerRemoteSpawning
  `/player`によってbotを遠隔で召喚できるプレイヤーを指定する。ここでいう遠隔とは、16m以上離れた場所もしくは別のディメンションにスポーンさせることを指す。
  + 初期値 : `true`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + carpet / [player](./carpet.html#player)
### farmlandTrampledDisabled
  耕地がmobやplayerの踏み荒らしによって土へと戻る仕様を無効にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [turtleEggTrampledDisabled](#turtleeggtrampleddisabled)
### fillCommandModeEnhance
  `/fill`コマンドに`softreplace`モード
  を追加する。`<softreplae>`は置換前のブロックの状態をできるだけ維持するようにする。たとえば階段やハーフのブロックタイプのみを入れ替えたい場合に有効手となる。
  + 初期値 : `true`
  + 使用できる値 : `true` `false`
### flattenTriangularDistribution
  minecraftのランダマイザーを三角分布から一様分布に変更する。よりエッジケースが多く起こる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### fluidDestructionDisabled
  流体によるブロックの破壊を無効にする。流体は本来破壊されるべきブロックも破壊されないブロックとして扱うになる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### hopperCountersUnlimitedSpeed
  `/counter`によって有効になったカウンタのホッパーとしてのクールダウンを無効にする。hopperCountersが有効になっている場合にのみ動作する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [hopperCounter](./carpet.html#hoppercounters)
    + carpet / [counter](./carpet.html#counter)
### hopperNoItemCost
  `/scounter`を有効にする。詳しくは[scounter](#scounter)を参照。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [scounter](#scounter)
### HUDLoggerUpdateInterval
  HUDとして表示されるloggerの更新頻度を変更する。単位はgtで、全てのloggerに対して適用される。
  + 初期値 : `20`
  + 使用できる値 : `integer`
  + 関連項目
    + carpet / [log](./carpet.html#log)
### instantBlockUpdaterReintroduced
  update suppressorを1.19+で使用可能にする。さらにmicrotiming loggerをより見やすい形で提供するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [updateSuppressionSimulator](#updatesuppressionsimulator)
    + [yeetUpdateSuppressionCrash](#yeetupdatesuppressioncrash)
    + carpet / [updateSuppressionBlock](./carpet.html#updatesuppressionblock)
### instantCommandBlock
  レッドストーン鉱石の上におかれたコマンドブロックはtileTickでscheduleすることによる1gtの遅延がなく、インスタントに起動する。ノーマルコマンドブロックのみが影響を受ける。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### itemEntitySkipMovementDisabled
  itemは接地判定を4gt毎に行っているが、これを1gt毎にする。いくつかの回路が壊れる可能性がある。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### keepMobInLazyChunks
  lazy chunk内に存在するmobはデスポーンしなくする。1.15と1.16でのみ有効。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### largeBarrel
  最適なstorage block。樽の横に並べて底面を合わせるとラージチェストのように一つの大きな樽として機能する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### lifeTimeTrackerConsidersMobcap
  lifetimeの計測がmobcapにカウントされないmobを考慮するようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [lifetime](#lifetime)
### lightQueueLoggerSamplingDuration
  light queueのloggerのサンプルレートを指定する。
  + 初期値 : `60`
  + 使用できる値 : `integer`
### lightUpdates
  light updateに関するシミュレートをするようにする。
  `on`にするとバニラ同様に処理される。

|              | light update | schedule |
|:-------------|:---:|:---:|
| `on`         |  O  |  O  |
| `off`        |  X  |  X  |
| `suppressed` |  X  |  O  |
| `ignored`    |  O  |  X  |

  <div class="md-warning">

  `off`もしくは`suppressed`を指定すると、新しいチャンクが読み込まれなくなる。この状態で新しいチャンクを読み込もうとするとサーバーが恒常的なスタックを引き起こす。
  </div>

  + 初期値 : `on`
  + 使用できる値 : `on` `off` `suppressed` `ignored`
### loggerMovement
  `/log movement`を使用できるプレイヤーを指定する。
  + 初期値 : `ops`
  + 使用できる値 : `true` `false` `ops` `0` `1` `2` `3` `4`
  + 関連項目
    + carpet / [log](./carpet.html#log)
### microTiming
  `/log microtiming`を有効にする。レッドストーン・コンポーネントのアクション、blockUpdate、stack traceを染料アイテムでログに記録し、表示する。dye markerの使い方については[microTimingDyeMarker](#microtimingdyemarker)を参照。またlogのメソッドの変更については[microTimingTarget](#microtimingtarget)を参照。
  <div class="md-note">
  有効にすると、パフォーマンス面で甚大な影響を及ぼす可能性がある。
  </div>

  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [microTimingDyeMarker](#microtimingdyemarker)
    + [microTimingTarget](#microtimingtarget)
    + [microTimingTickDivision](#microtimingtickdivision)
    + [log](#log)
### microTimingDyeMarker
  染料を持った状態でブロックを右クリックすることでlogに表示するmicro timingの表示をするブロックを選択できるようにする。また、染料に名前をつけることで表示させる名前を変更することができる。

  ブロックをマークするには`/log microtiming`を表示させる必要がある。もう一度選択することでblockUpdateをマークできる。さらにもう一度選択することでマーカーを削除できる。

  スライムボールで右クリックすることで対応するブロックが移動したときにlogに出す座標も移動させるようにすることができる。

  `clear`とすることですべてのマーカーを削除できる。

  クライアントにcarpetが導入されている場合、マーキングされたブロックがボックスで表示される。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `clear`
  + 関連項目
    + [microTiming](#microtiming)
    + [microTimingTarget](#microtimingtarget)
    + [microTimingTickDivision](#microtimingtickdivision)
### microTimingTarget
  micro timingに記録するイベントの指定方法を変更する。ただし染料マーカーが付いたイベントは常にログに記録される。<br>
  `labelled` : 羊毛でラベル付けされたものを記録する。**非推奨**。<br>
  `in_range` : 全てのプレイヤーの半径32m以内のものについて記録する。**非推奨**。<br>
  `all` : 全て記録する。**非推奨**。<br>
  `marker_only` : 染料マーカーのみ。
  + 初期値 : `marker_only`
  + 使用できる値 : `labelled` `in_range` `all` `marker_only`
  + 関連項目
    + [microTiming](#microtiming)
    + [microTimingDyeMarker](#microtimingdyemarker)
    + [microTimingTickDivision](#microtimingtickdivision)
### microTimingTickDivision
  micro timingの記録の分割地点を指定する。
  `world_timer`で実質的にgametickで分割され、`player_action`でプレイヤーによる変更によって分割される。
  + 初期値 : `world_timer`
  + 使用できる値 : `world_timer` `player_action`
  + 関連項目
    + [microTiming](#microtiming)
    + [microTimingDyeMarker](#microtimingdyemarker)
    + [microTimingTarget](#microtimingtarget)
### minecartFullDropBackport
  トロッコがアイテムになるとき、コンポーネントとトロッコで分離せずコンポーネントつきトロッコとしてドロップする仕様をバックポートする。minecraft <1.19で有効。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### minecartTakePassengerMinVelocity
  トロッコがmobを乗せるために必要な最小水平速度(m/gt)を指定する。
  `0`に指定するとボートのように静止していても常にmobを乗せることができる。
  `NaN`に指定すると一切乗せなくなる。
  + 初期値 : `0.1`
  + 使用できる値 : `NaN` `double`
### mobcapsDisplayIgnoreMisc
  mobcapsから~~存在するだけでなにもしない哀れな~~`misc`を除外する。`log`と`/spawn mobcaps`に影響を与える。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [log](./carpet.html#log)
    + carpet / [spawn](./carpet.html#spawn)
### oakBalloonPercent
  オークの木が条件を満たした時巨木になる確率をパーセンテージで指定する。負の数を指定することでバニラ準拠にできる。値は0~100もしくは負の数でなければならない。
  + 初期値 : `-1`
  + 使用できる値 : `0 ~ 100` `-1`
### observerNoDetection
  オブザーバーがstateUpdateを検知しなくする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### opPlayerNoCheat
  opをもったプレイヤーでもチートができないようにする。
  + 影響を受けるコマンド
    + `/gamemode`
    + `/tp`
    + `/teleport`
    + `/give`
    + `/setblock`
    + `/summon`
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### optimizedFastEntityMovement
  エンティティのモーメンタムを現在移動している軸のブロックの当たり判定のみに限定して確認することで最適化を図るようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### optimizedHardHitBoxEntityCollision
  硬い当たり判定をもつボートとシュルカーについて、多くの不必要な反復処理を省くことで最適化を図るようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### optimizedTNTHighPriority
  carpetのoptimizedTNTがlithiumの爆発物の最適化を上書きできるようにする。`optimizedTNT`が有効でないと動作しない。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [optimizedTNT](./carpet.html#optimizedtnt)
### poiUpdates
  ブロックの変更によってPOI updateを起こさないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### persistentLoggerSubscription
  logを再ログイン後も切断時と同じ状態になるようにする。最初のログイン時のみdefaultLoggerを適用するようにする。
  誰がなにを記録しているのかは`config/carpettisaddition/logger_subscriptions.json`に保存される。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [log](./carpet.html#log)
### preciseEntityPlacement
  itemによってエンティティを配置、召喚するとき、正確にカーソルの位置に配置されるようにする。
  + 影響を受けるアイテム
    + 防具立
    + エンドクリスタル
    + スポーンエッグ
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### railDupingFix
  レールの複製を修正する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [sandDupingFix](#sanddupingfix)
    + [tntDupingFix](#tntdupingfix)
### redstoneDustRandomUpdateOrder
  レッドストーンダストの更新順を座標依存ではなくランダムにする。座標依存を調べる場合に有用。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### renewableDragonEgg
  ドラゴンの卵がドラゴンブレスにあたったとき、ドラゴンの卵が新しく生成されるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [dispensersFireDragonBreath](#dispensersfiredragonbreath)
### renewableDragonHead
  エンダードラゴンが帯電クリーパーによって殺されたとき、ドラゴンの頭を落とすようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### renewableElytra
  ファントムがシュルカーによって殺されたとき、低い確率でエリトラを落とすようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### repeaterHalfDelay
  レッドストーン鉱石の上におかれたリピーターは通常の1/2の遅延になるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### sandDupingFix
  砂を含めた重力の働くブロックの複製がされないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [railDupingFix](#raildupingfix)
    + [tntDupingFix](#tntdupingfix)
### snowMeltMinLightLevel
  雪のレイヤーがrandom tickによって融解する最小のlight levelを指定する。雪が積もる最大のlight levelである`10`を指定するとsnow proofを検証することができる。
  + 初期値 : `12`
  + 使用できる値 : `integer`
### stopCommandDoubleConfirmation
  サーバーを閉じるためには`/stop`を1分間に2回入力しないととじれないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### structureBlockDoNotPreserveFluid
  すでに水がおかれていてストラクチャーブロックによってwaterlogged可能なブロックが設置されるときに、waterloggedが`true`にならないようにする。

  [MC-130584](https://bugs.mojang.com/browse/MC-130584)を修正する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [structureBlockIgnored](./carpet.html#structureblockignored)
    + carpet / [structureBlockLimit](./carpet.html#structureblocklimit)
    + carpet / [structureBlockOutlineDistance](./carpet.html#structureblockoutlinedistance)
### synchronizedLightThread
  light levelを計算するlight engineが利用するlight threadをtickに同期させる。1.20以降light engineが大幅に変更され軽量化が施された結果非同期となることはほぼなくなったが、tickの最初にlight threadをまつようになる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### syncServerMsptMetricsData
  `alt+F3`によってみれるmsptの表示を実際のmsptと同期させる。クライアントにcarpet TIS additionが必要。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tileTickLimit
  1gt内でおこすことができるtileTickのschedule limitを指定する。値は1以上である必要がある。
  + 初期値 : `65536`
  + 使用できる値 : `integer`
### ~~tiscmNetworkProtocol~~
  tiscmのプロトコルに関するスイッチ。ところでtism network protocolってなに。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tntDupingFix
  掘れ。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [railDupingFix](#raildupingfix)
    + [sandDupingFix](#sanddupingfix)
### tntIgnoreRedstoneSignal
  tntがレッドストーンの信号によって発火しないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### tntFuseDuration
  tntの発火の遅延を指定する。単位はgt。
  + 初期値 : `80`
  + 使用できる値 : `integer`
### tooledTNT
  tntを着火した人のメインハンドの効果がtntに付与されるようにする。たとえばシルクタッチのつるはしを持っていてtntが氷を壊した場合、氷はドロップする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### totallyNoBlockUpdate
  完全にblockUpdateとstateUpdateを発生しなくする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [fillUpdates](./carpet.html#fillupdates)
    + carpet / [tntDoNotUpdate](./carpet.html#tntdonotupdate)
### toughWitherRose
  wither roseをどこにでも植えられるようになる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### turtleEggTrampledDisabled
  亀の卵を踏み荒らし破壊することを無効にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [farmlandTranmledDisabled](#farmlandtrampleddisabled)
### undeadDontBurnInSunlight
  アンデッドmobは日光によって燃えないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### updateSuppressionSimulator
  レッドストーン鉱石の上におかれたパワードレールもしくはアクティベータレールは`powered`が`true`から`false`になる直前に指定したJVM例外処理を投げるようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false` `StackOverflowError` `OutOfMemoryError` `ClassCastException`
  + 関連項目
    + [yeetUpdateSuppressionCrash](#yeetupdatesuppressioncrash)
    + carpet / [UpdateSuppressionBlock](./carpet.html#updatesuppressionblock)
### visualizeProjectileLoggerEnabled
  projectile loggerを可視化する。従来の表示形式ではなく、その場所に小さいエンティティをマーカーとして表示させることでより見やすくさせる。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + carpet / [log](./carpet.html#projectiles)
### voidDamageAmount
  奈落のダメージ量を変更する。
  + 初期値 : `4`
  + 使用できる値 : `double`
  + 関連項目
    + [voidDamageIgnorePlayer](#voiddamageignoreplayer)
    + [voidRelatedAltitude](#voidrelatedaltitude)
### voidDamageIgnorePlayer
  プレイヤーは奈落ダメージを受けないようにする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
  + 関連項目
    + [voidDamageAmount](#voiddamageamount)
    + [voidRelatedAltitude](#voidrelatedaltitude)
### voidRelatedAltitude
  ワールドの底から奈落ダメージを受け始める高さまでの差分を設定する。単位はblock。
  + 初期値 : `-64`
  + 使用できる値 : `double`
  + 関連項目
    + [voidDamageAmount](#voiddamageamount)
    + [voidDamageIgnorePlayer](#voiddamageignoreplayer)
### witherSpawnedSoundDisabled
  witherのスポーンする音を無効にする。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
### ported-rules
ほかのmodから移植されたrule。TISなりの変更が加えられている場合がある。
<details>
  <summary>ported rules</summary>

#### lightEngineMaxBatchSize
  light engineの最大バッチサイズをオーバーライドする。値は正の数でなければならない。
  + 初期値 : `5`
  + 使用できる値 : `double`
  + 関連項目
    + [lightUpdates](#lightupdates)
#### yeetUpdateSuppressionCrash
  update supressionによるクラッシュを防ぐ。またクラッシュしようとした場合その原因をlogに出力する。
  + 初期値 : `false`
  + 使用できる値 : `true` `false`
</details>

## command
独自のコマンドもあるが、carpetのコマンドに変数を追加することも多い。その場合追加分のみを記載するが、関連項目よりほかの選択肢も見ることができる。
### info
`/info world [ticking_order | weather]`を追加する。ワールドに関する情報を表示する。また、`/info entity`を利用可能にする。さらに`/info block`にtick eventとblock eventの情報を追加する。
+ `[ticking_order | weather]`
  + `ticking_order`<br>
    ディメンションの処理順を表示する。技術的には同じ鯖でマルチワールドを導入している場合、ワールドの処理順も表示することができるとされている。
  + `weather`<br>
    天候と天気予報を表示する。
+ 関連項目
  + carpet / [info](./carpet.html#info)
  + carpet / [commandInfo](./carpet.html#commandInfo)
### lifetime
`/lifetime [help | filter | tracking | <entity_type>]`で使用できる。特定のエンティティのスポーン/削除に関する情報を表示する。すべてにおいて、`realtime`を最後に挿入した場合、計算がtickベースからhourベースになる。
+ `[help | filter | tracking | [entity_type]]`
  + `help`<br>
    このコマンドに対するヘルプを表示する。[complete doc](https://github.com/TISUnion/Carpet-TIS-Addition/blob/master/docs/commands.md#lifetime)がでてくる。
  + `tracking`<br>
    `/lifetime tracking <start | stop | restart>`で利用可能。アクションを選択しなかった場合、データがある場合現在の情報を表示する。
  + `filter`<br>
    `/lifetime filter [entity_type] [set | clear] [target]`でtrackingするエンティティを指定する。`[entity_type]`は全てのmobEntityとitemEntity、experienceOrbが指定可能。`[target]`のfilterに`[set | clear]`でセットもしくはクリアができる。`[entity_type]`と`[target]`には`@e[type=zombie,distance=..100]`などのターゲットセレクタを用いて指定できる。
  + `<entity_type>`<br>
    `/lifetime [entity_type] <lifetime | removal | spawning>`で利用できる。`<entity_type>`に関するより詳細な情報を表示する。指定しなかった場合そのすべてを表示する。
    + `lifetime`<br>
      の生存時間の最小、最大、平均を表示する。さらに最後のエンティティのスポーンした座標と削除された座標を、それぞれ<font color=green>[S]</font>と<font color=crimson>[R]</font>をホバーすることで表示できる。クリックすることでtpするコマンドが生成される。
    + `spawning`<br>
      そのエンティティがスポーンした理由とその数、効率を表示する。
    + `removal`<br>
      そのエンティティが削除された理由とその数、効率を表示する。
+ トラッキングできること
  <details>
    <summary>スポーンした理由</summary>
          
    + Natural spawning
    + Nether portal pigman spawning
    + /summon command
    + Spawned by item
    + Block drop (item only)
    + Dropped from container (item only)
    + Slime division
    + Zombie Reinforce
    + Spawned by spawner
    + Spawned in raid as raider
    + Be summoned by entity or block
    + Breeding
    + Dispensed by block
    + Mob drop (item and xp orb only)
    + Mob throw (item only)
    + Dismounts from a vehicle (1.16+)<br>
      [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)が`true`であることを要求
    + Enderman placed down a block (1.16+)<br>
      [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)が`true`であることを要求
    + Mob conversion
    + Trans-dimension from portal
  </details>
  <details>
    <summary>削除された理由</summary>

    + Despawn<br>
      immediately despawn、random despawn、difficulty despawn、timeout despawnを含む。
    + Damaged to death
    + Becomes persistent<br>
      [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)が`true`であることを要求
    + Rides on a vehicle (1.16+)<br>
      [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)が`true`であることを要求
    + Enderman picked up a block (1.16+)<br>
      [lifeTimeTrackerConsidersMobcap](#lifetimetrackerconsidersmobcap)が`true`であることを要求
    + Entity merged (item and xp orb only)
    + Collected up by hopper or hopper minecart (item only)
    + Entering void
    + Self-exploded
    + Picked up by player or mob (item and xp orb only)
    + Mob conversion
    + Trans-dimension through portal
    + Other<br>
      もしほかの理由をトラッキングしたい場合、issueをあげれば対応するとのこと。
  </details>
+ 関連項目
  + [commandLifetime](#commandlifetime)
  + [log](#log)
### log
carpetの[log](./carpet.html#log)に様々な`[subject]`を追加する。また、`/log [loggerName] <option> [player]`および`/log clean [player]`にopレベル2を要求するようにする。
+ `[subject]`
  + `commandBlock`
  + `damage`
  + `item`
  + `lifetime`
  + `lightQueue`
  + `memory`
  + `microTiming`
  + `mobcapsLocal`
  + `movement`
  + `phantom`
  + `raid`
  + `scounter`
  + `ticket`
  + `tickWarp`
  + `turtleEgg`
  + `xporb`
+ 関連項目
  + carpet / [log](./carpet.html#log)
<details>
<summary>subject</summary>

+ commandBlock<br>
  `/log commandBlock <throttled | all>`でコマンドブロックもしくはコマンドブロック付きトロッコがいつどこでどのようなコマンドを実行したのかを表示する。

  また、表示されたコマンドに対して<font color=crimson>[X]</font>をクリックすることでそのコマンドブロックもしくはエンティティを削除するコマンドを生成する。
  + `<throttled | all>`<br>
    指定しない場合、throttledが指定される。
    + `throttled`<br>
      三秒毎に一番最近実行されたコマンドを表示する。
    + `all`
      毎gt表示する。
  + 表示場所<br>
    チャット
+ damage<br>
  `/log damage <option>`でどのエンティティがどのエンティティにどれだけのダメージをどのように与えようとして、実際はどれだけのダメージ量でどれだけHPが残っているのかを表示する。
  + `[option]`<br>
    どのダメージを表示するかを指定する。詳細は[英語doc]を参照。指定しない場合全てのダメージを表示する。
    + `"<entityA>-><entityB>"`<br>
      `<entityA>`から`<entityB>`に対してのダメージのみを記録する。`<entityA>`および`<entityB>`を指定しなかった場合それぞれ全てを指定したものとする。`"<entityA><-><entityB>"`とするとどちらの場合でも表示する。

      エンティティの指定にはターゲットセレクタを用いることもでき、複数選択が可能である。
    + `<entity_selector>`<br>
      そのエンティティに関するダメージを表示する。ターゲットセレクタを利用する場合複数選択可能で、`players`とするとプレイヤーに関するダメージを表示する。`zombie`のようにエンティティIDを使うことで省略することもできる。ただしopレベル2を要求する。
    + `me`<br>
      自身に関するダメージを表示する。`entity_selector`で`@s`とするのと同義。
    + `all`<br>
      全てを表示する。
  + 表示場所<br>
    チャット
+ item<br>
  `/log item <create | die | despawn>`でitemに対して例えばデスポーンなどなにかがおきたときにそれの情報を表示する。
  + `<create | die | despawn>`<br>
    それぞれを`,`でつなぐことで二つ以上のオプションを指定できる。
    + `create`<br>
      アイテムエンティティがワールドに生成されたときそのstack traceと理由とともに表示する。
    + `die`<br>
      時間経過によるデスポーンではなく、ダメージを受けて消滅したときに表示する。
    + `despwan`<br>
      アイテムが時間経過によってデスポーンしたときに表示する。
  + 表示場所<br>
    チャット
+ lifetime<br>
  `/lifetime <entity_type>`現在プレイヤーがいるディメンションでライフタイムトラッカーによって記録されている特定のエンティティについてその統計を表示する。
  + `<entity_type>`<br>
    全てのトラッキングされているエンティティが有効。指定しなかった場合全てのエンティティを指定したものとされる。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + [lifetime](#lifetime)
+ lightQueue<br>
  `/log lightQueue <dynamic | dimension>`によって今のライトキューのサイズ、どれだけライトサプレッサーの推定使用可能時間、ライトキューの生成速度、処理速度を表示する。それぞれは
  + `<dynamic | dimension>`<br>
    指定しなかった場合`dynamic`が指定される。
    + `dynamic`<br>
      現在表示させているプレイヤーがいるディメンションを表示する。
    + `dimension`<br>
      特定のディメンションについて表示する。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + [lightQueueLoggerSamplingDuration](#lightqueueloggersamplingduration)
    + [lightEngineMaxBatchsize](#lightenginemaxbatchsize)
+ memory<br>
  `/log memory`現在サーバーが占有しているRAMサイズを表示する。`Used memory / Allocated memory | Max memory`で表示される。
  + 表示場所<br>
    プレイヤーリスト
+ microTiming<br>
  `/log microTiming <type>`でレッドストーンコンポーネントのマイクロタイミングを表示する。表示するコンポーネントがあるチャンクはチケットレベルが32以下でなければならない。
  + `<type>`<br>
    指定しなかった場合`merged`が指定される。
    + `all`<br>
      全てのイベントについて表示する。
    + `merged`<br>
      同じイベントは同じものとして表示される。
    + `unique`<br>
      毎gt固有のイベントについて表示する。
  + 表示場所<br>
    チャット
  + 関連項目
    + [microTiming](#microtiming)
+ mobcapsLocal<br>
  `/log mobcapsLocal [player]`で`[player]`まわりに発生するmobcapsを表示させる。minecraft 1.18.2+で利用可能。
  + `[player]`<br>
    全てのオンラインのプレイヤーが利用可能。指定したあとオフラインになった場合そのプレイヤーは存在しないと表示される。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目<br>
    + [mobcapsDisplayIgnoreMisc](#mobcapsdisplayignoremisc)
+ movement<br>
`/log movement <target>`で`<target>`がどれだけ移動しようとして、実際にどれだけ移動したかを表示する。
  + `<target>`<br>
    ターゲットセレクタによって複数指定することができる。ただし適切に選択しなければログのスパムおよびラグの原因になる。
    指定しなかった場合`non_zero:@a[distance..10]`が指定されるが、opレベルがたりない場合実行できない。

    <div class="md-note">
    指定するときに`non_zero:`を初めにくわえることで0ベクトルになったものは表示されなくなる。
    </div>
  
  + 表示場所<br>
    チャット
  + 関連項目
    + [loggerMovement](#loggermovement)
+ phantom<br>
  `/log phantom <spawning | reminder>`でファントムのスポーンに関する変更をする。
  + `<spawning | reminder>`<br>
    選択しなかった場合`spawning`が選択される。`"spawning,reminder"`とすることで両方を指定することができる。
    + `spawning`<br>
      だれかがファントムをスポーンさせたらそれを知らせる。
    + `reminder`<br>
      だれかが45分もしくは60分寝なかった場合お知らせする。
  + 表示場所<br>
    チャット
+ raid<br>
  `/log raid`によって襲撃の作成、無効化、bad omen levelの増加、そしてセンターの移動情報を表示する。
  + 表示場所<br>
    チャット
  + 関連項目
    + [raid](#raid)
+ scounter<br>
  `/log scounter <color>`でサプライカウンタの効率を表示する。
  + `<color>`<br>
    16色が利用可能。指定しなかった場合有効なものを表示する。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + [hopperNoItemCost](#hoppernoitemcost)
    + [scounter](#scounter)
+ ticket<br>
  `/log ticket <type>`でminecraftのチケットが作成され削除されたとき表示する。
  + `<type>`<br>
    `,`を使ってつなげることで複数の値を選択できる。指定しなかった場合`poartal`が選択される。
    + `portal`
    + `dragon`
    + `start`
    + `player`
    + `forced`
    + `light`
    + `post_teleport`
    + `unknown`

    <div class="md-warning">
    unknown ticketはスパム判定をもらう可能性がある。
    </div>

  + 表示場所<br>
    チャット
+ tickWarp<br>
  `/log tickWarp <option>`で現在のtickWarpのステータスを表示する。tickWrapが行われていない場合表示されない。`/tick warp status`よりは情報量がすくない。
  + `<option>`<br>
    指定しなかった場合`bar`が指定される。
    + `bar`<br>
      バー形式で表示する。
    + `value`<br>
      値を表示する。
  + 表示場所<br>
    プレイヤーリスト
  + 関連項目
    + [tick](#tick)
+ turtleEgg<br>
  `/log turtleEgg`で亀の卵がいつ踏みつぶされたかを表示する。
  + 表示場所<br>
    チャット
+ xporb<br>
  `/log xporb <create | die | despawn>`でexperience_orbに対して例えばデスポーンなどなにかがおきたときにそれの情報を表示する。
  + `<create | die | despawn>`<br>
    それぞれを`,`でつなぐことで二つ以上のオプションを指定できる。
    + `create`<br>
      アイテムエンティティがワールドに生成されたときそのstack traceと理由とともに表示する。
    + `die`<br>
      時間経過によるデスポーンではなく、ダメージを受けて消滅したときに表示する。
    + `despwan`<br>
      アイテムが時間経過によってデスポーンしたときに表示する。
  + 表示場所<br>
    チャット
</details>

### manipulate
`/manipulate [container | entity]`で世界を操作する。
+ `[container | entity]`
  + `container`<br>
    `/manipulate container [data] [operation]`でコンテナの`[data]`を`[operation]`に従って操作する。
    <details>
      <summary>操作とコマンドリスト</summary>
      <table>
      <thead>
      <tr>
      <th align="center">container name</th>
      <th align="center">[data]</th>
      <th align="left">[operation]</th>
      </tr>
      </thead>
      <tbody>
      <tr>
      <td align="center">Entity list</td>
      <td align="center"><code>entity</code></td>
      <td align="left"><code>revert</code> <code>shuffle</code></td>
      </tr>
      <tr>
      <td align="center">Tickable tile entity list</td>
      <td align="center"><code>tileentity</code></td>
      <td align="left"><code>revert</code> <code>shuffle</code> <code>querry</code> <code>statistic</code></td>
      </tr>
      <tr>
      <td align="center">Tile tick queue</td>
      <td align="center"><code>tiletick</code></td>
      <td align="left"><code>add</code> <code>remove</code></td>
      </tr>
      <tr>
      <td align="center">Block event queue</td>
      <td align="center"><code>blockevent</code></td>
      <td align="left"><code>add</code> <code>remove</code></td>
      </tr>
      </tbody>
      </table>
    <pre><code>
    /manipulate container entity [revert | shuffle]
    /manipulate container tileentity [query | revert | shuffle | statistic]
    /manipulate container tiletick add [pos] [block] [delay] [<priority>]
    /manipulate container tiletick remove [pos]
    /manipulate container blockevent add [pos] [block] [type] [data]
    /manipulate container blockevent remove [pos]
    </code></pre>
    たとえば<code>/manipulate container tileentity shuffle</code>を使用すると、タイルエンティティは通常設置した順に処理されるが、この順番をランダムにさせることができる。これにより依存を調べることが可能になる。
    </details>

  + `entity`<br>
    `/manipulate entity [target] [operation]`で`[target]`を`[operation]`に従って操作する。詳細は後述。

    `[target]`はminecraftのターゲットセレクタによって指定することも可能だが、対象は必ず一つでなければならない。
        
    <div class="md-note">

    複数の可能性がある対象の指定をする場合には、例えば`@e[sort=nearest,limit=1]`とすることで対象を一つに絞ることができる。
    </div>
    <details>
    <summary>コマンド</summary>
      
    customNameを変更もしくは削除する。 
    ```
    /manipulate entity [target] rename <text>
    /manipulate entity [target] rename clear
    ```
    persistentタグを変更する。つまり、自然にデスポーンするかを変更することができる。
    ```
    /manipulate entity [target] persistent [true | false]
    ```
    エンティティに乗せる、もしくはエンティティからおろす。
    ```
    /manipulate entity [target] mount <vehicle>
    /manipulate entity [target] dismount
    ```
    エンティティに対して速度を与える。
    ```
    /manipulate entity [target] velocity [add | set] [x] [y] [z]
    ```
    </details>

+ 関連項目
  + [commandManipulate](#commandmanipulate)
### player
`/player`の`[conduct]`に`randomly`、`after`および`perTick`を追加する。
+ `[conduct]`
  + `randomly`<br>
    `/player [mcid] [action] randomly [method] [method_option]`によって`[method]`と`[method_option]`に基づいてランダムに指定の行動をとる。テストをする場合、`[method_option]`に`--simulate`を追加する。

    `[method]`を指定しないとヘルプが出る。
    + `[method]`<br>
      全ての値の単位はgt。
      + `gaussian`<br>
        いわゆる正規分布もしくはガウス分布。`[method_option]`には\\( μ \\)および\\( σ \\)をこの順で指定する。
        <details>
        <summary>gaussian</summary>
        平均を\\( μ \\)、分散を\\( σ^2>0 \\)とするとき、確率密度関数\\(f(x)\\)が以下の式

        $$ f(x)=\frac{1}{\sqrt{π\sigma^2}}\exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right) $$

        で与えられる確率分布。
        </details>

      + `poisson`<br>
        いわゆるポアソン分布。
      + `uniform`<br>
        最小値と最大値をこの順で指定するとその間の数値で一様に選出する。
  + `after`<br>
    `/player [mcid] [action] after [count]`でコマンド実行後から`[counter]`gt後にその動作が実行される。
  + `perTick`<br>
    `/player [mcid] [action] perTick [count]`で1gtの間に`[count]`回その動作を実行する。`[count]`の値は1から64までをとる。
+ 関連項目
  + carpet / [player](./carpet.html#player)

### raid
`/raid [list | tracking]`で襲撃に関する情報を表示する。
+ `[list | tracking]`
  + `list`<br>
    `/raid list <full>`で現在発生している襲撃に関する情報を表示する。`<full>`を挿入した場合、省略されている情報をすべて表示する。
  + `tracking`<br>
    `/raid tracking <start | stop | restart | realtime>`でraidの統計をとる。`realtime`を指定すると計算がtickベースからhourベースになる。なにも挿入しなかった場合記録されているデータを表示する。
+ 関連項目
  + [commandRaid](#commandraid)
### raycast
`/raycast [coordinate-1] [coordinate-2] <shapeMode> <fluidMode>`で`[coordinate-1]`から`[coordinate-2]`まで直線を描き、ぶつかったブロックとその座標を表示する。もし何一つぶつからなかった場合<font color=crimson>Raycast missed</font>と表示される。
<div class="md_note">

  `[coordinate-1]`と`[coordinate-2]`が離れすぎている場合、tickがしばらく止まる場合がある。
</div>

+ `<shapeMode>`
  + `collider` (default value)
  + `outline`
  + `visual` (mc1.16+)
  + `falldamage_resetting` (mc1.18.2+)
+ `<fluidMode>`
  + `none` (default value)
  + `source_only`
  + `any`
  + `water` (mc1.18.2+)
+ 関連項目
  + [commandRaycast](#commandraycast)
### reflesh
`/reflesh [inventory | chunk]`でインベントリもしくはチャンクを更新する。
+ `[inventory | chunk]`
  + `inventory`<br>
    `/reflesh inventory <target>`で`<target>`のインベントリを更新する。自分以外のエンティティを指定する場合opレベル2が必要。
  + `chunk`
    `/reflesh chunk [location]`で`location`にあるチャンクを更新する。
    |`[location]`|`chunk`|
    |:---:|---|
    |`all`|読み込まれているすべてのチャンク|
    |`at`|特定の1チャンク、チャンク座標を用いて`at [X] [Z]`の形式で指定する|
    |`current`|現在の座標を含む1チャンク|
    |`inrange`|チェビシェフ距離を用いた範囲内にある全てのチャンク|
+ 関連項目
  + [commandReflesh](#commandrefresh)
### remoteentity
`/removeentity [target]`で`[target]`をワールドから直接削除する。複数選択が可能であるが、プレイヤーは影響しない。
<div class="md-important">

似たコマンドである`/removeabove` `/removebelow` `/removenear`は全てWorldEditによるものである。
</div>

+ 関連項目
  + [commandRemoverntity](#commandremoveentity)
### scounter
ホッパーの上に羊毛を置いて中にアイテムをいれることで、そのアイテムを無限に供給するようにする。ただし自身以外によってインベントリからアイテムが取り除かれた場合は供給されなくなる。

`/scounter <color> <realtime | reset>`で情報を表示する。
+ `<color>`<br>
  割愛。色を使い分けることでチャンネルを湧けることができる。16色16チャンネルを同時に扱える。複数選択はできない。指定しなかった場合現在有効な全てのチャンネルを指定したものとする。
+ `<reset | realtime>`<br>
  指定しなかった場合`<color>`で指定したチャンネルの効率を表示する。
  + `reset`<br>
    `<color>`で指定したチャンネルをリセットする。
  + `realtime`<br>
    効率の計算をtickベースからhourベースに変更して表示する。
+ 関連項目
  + [hopperNoItemCost](#hoppernoitemcost)
  + carpet / [hopperCounter](./carpet.html#hoppercounter)
  + carpet / [counter](./carpet.html#counter)
### sleep
`/sleep [duration] [unit]`でこのコマンド実行時から指定した時間ゲームを実行している**スレッド**に対してラグを発生させる。

[instantCommandBlock](#instantcommandblock)をtrueにすることで好きなタイミングで好きな時間だけラグを発生させることができる。

<div class="md-warning">
このコマンドはゲームを強制的に停止させるため、実行している間ほかのコマンドは受け付けないことに注意。
</div>
<div class="md-warning">
スレッドに対して行われるため同じスレッドで動いているプロセスも同様に処理が停止されるはずである。
</div>

+ `[duration]`<br>
  2147483647までの自然数。
+ `[unit]`<br>
  `[time]`の単位。`s` `ms` `us`が利用可能。それぞれ秒、ミリ秒、マイクロ秒である。
+ 関連項目
  + [commandSleep](#commandsleep)
### spawn
carpetの[spawn](./carpet.html#spawn)の`[subject]`に`mobcapsLocal`を追加する。
また、`/spawn tracking restart`を追加する。~~怠惰な奴め~~
+ `mobcapsLocal`<br>
  `/spawn mobcapsLocal [player]`で`[player]`によるmobcapを表示する。
+ 関連項目
  + carpet / [spawn](./carpet.html#spawn)
  + carpet / [commandSpawn](./carpet.html#commandspawn)
### tick
carpetの[tick](./carpet.html#tick)の`warp`に`status`を追加する。
+ `status`<br>
  `/tick warp status`によって現在の進捗を表示する。
+ carpet / [tick](./carpet.html#tick)
### script
スクリプトについては[TIS/misc/script](https://github.com/TISUnion/Carpet-TIS-Addition/blob/master/docs/misc.md#scarpet)を参照。~~説明できる自信がない~~

## update-logs
### latest
+ version : `v1.0.0`
+ TIS : `1.50.1`
+ 変更点
  + 誤字の訂正
+ 更新日<br>
  `23/10/16 UTC+9`
### previous
<details>
<summary>previous</summary>
<details>
<summary><code>v0.0.0</code></summary>

+ TIS : `1.50.1`
+ 変更点
  + ドキュメントの作成
+ 更新日<br>
  `2023/10/16 UTC+9`
</details>
</details>