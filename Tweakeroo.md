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