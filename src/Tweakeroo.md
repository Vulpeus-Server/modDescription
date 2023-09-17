<link href="Tweakeroo.css" rel="stylesheet"></link>

# TweakerooとTweakmoreの機能一覧
## 目次
# Tweakeroo
## Generic
### carpetAccuratePlacementProtocol
Carpet modを使用している場合に[`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)と[`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)を機能させる
+ 関連機能
  + [`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)
  + [`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)
### clientPlacementRotation
Carpet modが入っていない鯖またはシングルプレイで[`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)と[`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)を機能させる
+ 関連機能
  + [`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)
  + [`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)
### fastLeftClickAllowTools
ツールをメインハンドに所持している場合でも[`tweakFastLeftClick`](#tweakFastLeftclick)を機能させる
+ 関連機能
  +  [`tweakFastLeftClick`](#tweakFastLeftclick)
### fastPlacementRememberOrientation
[`tweakFastBlockPlacement`](`tweakFastBlockPlacement`)を使用したとき、最初に置いたブロックの向きを保存する
+ 関連機能
  +  [`tweakFastBlockPlacement`](#tweakFastBlockPlacement)
### freeCameraPlayerInputs
[`tweakFreeCamera`](#tweakFreeCamera)を使用している際に右クリックと左クリックを使用できるようにする
+ 関連機能
  + [`tweakFreeCamera`](#tweakFreeCamera) 
<!-- + 関連機能
  + [](#) -->
### freeCameraPlayerMovement
[`tweakFreeCamera`](#tweakFreeCamera)を使用している際にプレイヤーを移動させることができるようになる
>[!note]
>画面の移動はできないので見やすい位置に移動させたり、ホットキーに設定すること
+ 関連機能
  + [`tweakFreeCamera`](#tweakFreeCamera)
### handRestockPre
[`handRestockPreThreshold`](#handRestockPreThreshold)で設定した値までスタックできるアイテムが減った時、[`tweakHandRestock`](#tweakHandRestock)を発動させる
+ 関連機能
  + [`handRestockPreThreshold`](#handRestockPreThreshold)
  + [`tweakHandRestock`](#tweakHandRestock)
### hangableEntityBypassInverse
スニーク時に額縁や絵画をターゲットするかどうかを切り替える
|True/false|ターゲット|
|:--:|:--:|
|True|しない|
|False|する|
### itemUsePacketCheckBypass
1.18.2で追加された新たな距離・座標チェックを回避する。このチェックにより[`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)を有効化した状態で置いたブロックはゴーストブロックになり正しく機能しなくなる。
+ 関連機能
  + [`tweakAccurateBlockPlacement`](#tweakAccurateBlockPlacement)
+ 推奨される値:`true`
### permanentSneakAllowInGUIs
[`tweakPermanentSneak`](#tweakPermanentSneak)を有効にしている場合にGUI(インベントリなど)を開いてもスニークし続ける
+ 関連機能
  + [`tweakPermanentSneak`](#tweakPermanentSneak)
### placementRestrictionTiedToFast
[`tweakFastBlockPlacement`](#tweakFastBlockPlacement)のtrue/falseを切り替えたときに[`tweakPlacementRestriction`](#tweakPlacementRestriction)のtrue/falseも一緒に切り替える
+ 関連機能
  + [`tweakFastBlockPlacement`](#tweakFastBlockPlacement)
  + [`tweakPlacementRestriction`](#tweakPlacementRestriction)
+ 推奨される値:`true`
### potionWarningBeneficialOnly
[`tweakPotionWarning`](#tweakPotionWarning)で警告するポーションの効果を有益なもの(毒などのマイナスな効果以外の効果)だけにする
+ 関連機能
  + [`tweakPotionWarning`](#tweakPotionWarning)
+ 推奨される値:`true`
### rememberFlexibleFromClick
[`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)を使用中、最初に置いたブロックの状態を保存する。右クリックを離さずに次のブロックを置くと最初のブロックと同じ状態になる

+ 関連機能
  + [`tweakFlexibleBlockPlacement`](#tweakFlexibleBlockPlacement)
### shulkerDisplayBgColor
[`tweakShulkerBoxDisplay`](#tweakshulkerboxdisplay)でシュルカーボックスの中身を見たときのインベントリの色をシュルカーボックスの色と同じにする。Falseにするとプレイヤーのインベントリと同じ色が適用される
+ 関連機能
  + [`tweakShulkerBoxDisplay`](#tweakshulkerboxdisplay)
### shulkerDisplayRequireShift
[`tweakShulkerBoxDisplay`](#tweakshulkerboxdisplay)でシュルカーボックスの中身を覗くときにshiftキーを必要とするかどうか。Falseにするとカーソルを合わせるだけでシュルカーボックスの中身を覗くことができる
+ 関連機能
  + [`tweakShulkerBoxDisplay`](#tweakshulkerboxdisplay)
### slotSyncWorkaround
サーバーが[`tweakFastRightClick`](#tweakfastrightclick)などで高速使用されるアイテムの耐久値やスタック数をオーバーライドするのを防ぐ
### slotSyncWorkaroundAlways
[`slotSyncWorkaround`](#slotsyncworkaround)の適用範囲をTweakerooに存在する高速設置機能以外のmodの機能にも広げる。例えばLitematicaのEasy Place modeなど
### snapAimIndicator
[`tweakSnapAim`](#tweaksnapaim)を使用した際に表示されるインジケーターを表示するかどうか
+ 関連機能
  + [`tweakSnapAim`](#tweaksnapaim)
### snapAimOnlyCloseToAngle
[`tweakSnapAim`](#tweaksnapaim)でスナップが効く範囲を[`snapAimThresholdYaw`](#snapaimthresholdyaw)で設定した範囲にする。スナップする角度を変更するわけではないので注意。Falseにすると全ての角度でスナップする
+ 関連機能
  + [`tweakSnapAim`](#tweaksnapaim)
  + [`snapAimThresholdYaw`](#snapaimthresholdyaw)
### snapAimPitchOvershoot
[`snapAimMode`](#snapaimmode)を`Pitch`か`Yaw & Pitch`にした際にPitchの角度を`-90~90`から`-180~180`に変更する。化け物になりたい用設定
+ 関連機能
  + [`tweakSnapAim`](#tweaksnapaim)
  + [`snapAimMode`](#snapaimmode)
### zoomAdjustMouseSensitivity
[`tweakZoom`](#tweakzoom)でズーム中にマウスの感度を減少させる
+ 関連機能
  + [`tweakZoom`](#tweakzoom)
### blockTypeBreakRestrictionWarn
[`tweakBlockTypeBreakRestriction`](#tweakblocktypebreakrestriction)の警告文の表示位置を変更する
+ 関連機能
  + [`tweakBlockTypeBreakRestriction`](#tweakblocktypebreakrestriction)
+ 選択肢: `Message` `None` `Actionbar`
### breakingRestrictionMode
[`tweakBreakingRestriction`](#tweakbreakingrestriction)のモードを切り替える
+ 関連機能
  + [`tweakBreakingRestriction`](#tweakbreakingrestriction)
+ 選択肢: `Line` `Layer` `Diagonal` `Plane` `Face` `Column`
### elytraCameraIndicator
[`tweakElytraCamera`](#tweakelytracamera)を使用中に表示されるインジケーターの表示タイミングを切り替える。`With Key`では[`Hotkeys`](#hotkeys)タブの[`elytraCamera`](#elytracamera)で設定したキーを押したとき。 `Always`はずっと。 `Never`は表示しない。
+ 関連機能
  + [`tweakElytraCamera`](#tweakelytracamera)
  + [`elytraCamera`](#elytraCamera)
+ 選択肢: `With Key` `Always` `Never`
### entityTypeAttackRestrictionWarn
[`tweakEntityTypeAttackRestriction`](#tweakentitytypeattackrestriction)の警告文の表示位置を変更する
+ 関連機能
  + [`tweakEntityTypeAttackRestriction`](#tweakentitytypeattackrestriction)
  + 選択肢:`Message` `None` `Actionbar`
### placementRestrictionMode
[`tweakPlacementRestriction`](#tweakplacementrestriction)のモードを切り替える
+ 関連機能
  + [`tweakPlacementRestriction`](#tweakplacementrestriction)
  + `Line` `Layer` `Diagonal` `Plane` `Face` `Column`
### hotbarSwapOverlayAlignment
[`tweakHotbarSwap`](#tweakhotbarswap)が`True`のときに[`hotbarSwapBase`](#hotbarswapbase)で設定したキーを押下した際に表示されるオーバーレイの表示位置を変える
+ 関連機能
  + [`tweakHotbarSwap`](#tweakhotbarswap)
  + [`hotbarSwapBase`](#hotbarswapbase)
+ 選択肢:`Bottom Right` `Center` `Top Left` `Top Right` `Bottom Left`
### snapAimMode
[`tweakSnapAim`](#tweaksnapaim)のモードを切り替える
+ 関連機能
  + [`tweakSnapAim`](#tweaksnapaim)
+ 選択肢:`Yaw` `Pitch`
### chatTimeFormat
[`tweakChatTimestamp`](#tweakchattimestamp)を有効化した際に表示されるタイムスタンプのフォーマットを変更する
+ 関連機能
  + [`tweakChatTimestamp`](#tweakchattimestamp)
+ 初期値:`[HH:mm:ss]`