# carpet TIS addition
version : TIS 1.50.1

このドキュメント内では
`[]`を設定必須の値、`<>`を必須ではないが設定しなかった場合デフォルトの値が入力される値とする。
編集段階で未解決なものはストライクラインで示す。

以下はcarpetおよびそのaddonで日本語ドキュメントが存在もしくは作られる予定のリストである。

|mod|download|document|docs-JP|
|:---:|:---:|:---:|:---:|
|carpet|[modrinth](https://modrinth.com/mod/carpet)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet)<br>[github](https://github.com/gnembon/fabric-carpet)|[wiki](https://github.com/gnembon/fabric-carpet/wiki)|[carpet](./carpet.html)|
|carpet TIS addition|[modrinth](https://modrinth.com/mod/carpet-tis-addition)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-tis-addition)<br>[github](https://github.com/TISUnion/Carpet-TIS-Addition)|[docs](https://github.com/TISUnion/Carpet-TIS-Addition/tree/master/docs)|here|
|carpet extra|[modrinth](https://modrinth.com/mod/carpet-extra)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/carpet-extra)<br>[github](https://github.com/gnembon/carpet-extra)|[docs](https://github.com/gnembon/carpet-extra#carpet-mod-settings)||
|gugle-carpet-addition|[modrinth](https://modrinth.com/mod/gca)<br>[curseforge](https://www.curseforge.com/minecraft/mc-mods/guglecarpetaddition)<br>[github](https://github.com/Gu-ZT/gugle-carpet-addition)|[docs](https://github.com/Gu-ZT/gugle-carpet-addition#gca)|[GCA](gugle-carpet-addition.html)|



## 目次
<details>
  <summary>general</summary>

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

</details>


## general

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
    <code>off</code>もしくは<code>suppressed</code>を指定すると、新しいチャンクが読み込まれなくなる。この状態で新しいチャンクを読み込もうとするとサーバーが恒常的なスタックを引き起こす。
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
    + carpet / [log](./carpet.html#log)
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
  + 使用できる値 : `integer`
### observerNoDetection
  オブザーバーがstate updateを検知しなくする。
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
  carpetのoptimizedTNTがlithiumの爆発物の最適化を上書きできるようにする。とうぜん`optimizedTNT`が有効でないと動作しない。
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
