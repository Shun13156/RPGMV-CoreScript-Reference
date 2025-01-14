# Class: Window_Base

## Window_Base (x, y, width, height, _iconWidth, _iconHeight, _faceWidth, _faceHeight, _opening, _closing)

#### new Window_Base (x, y, width, height, _iconWidth, _iconHeight, _faceWidth, _faceHeight, _opening, _closing)

メッセージやステータスなどを描くためのメソッドを多く持つ、ウィンドウオブジェクト。<br />
[Window_EquipStatus](Window_EquipStatus.md), [Window_Gold](Window_Gold.md), [Window_Help](Window_Help.md), [Window_MapName](Window_MapName.md), [Window_Message](Window_Message.md), [Window_NameEdit](Window_NameEdit.md), [Window_ScrollText](Window_ScrollText.md), [Window_ShopStatus](Window_ShopStatus.md), [Window_SkillStatus](Window_SkillStatus.md) および [Window_Selectable](Window_Selectable.md) のスーパークラス。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | ウィンドウ x座標(ピクセル) |
| `y` | [Number](Number.md) | ウィンドウ y座標(ピクセル) |
| `width` | [Number](Number.md) | ウィンドウ幅(ピクセル) |
| `height` | [Number](Number.md) | ウィンドウ高さ(ピクセル) |
| `_iconWidth` | [Number](Number.md) | 基本のアイコン幅 規定値 : 32 |
| `_iconHeight` | [Number](Number.md) | 基本のアイコン高さ 規定値 : 32 |
| `_faceWidth` | [Number](Number.md) | 基本の顔画像の幅 規定値 : 144 |
| `_faceHeight` | [Number](Number.md) | 基本の顔画像の高さ 規定値 : 144 |
| `_opening` | Boolean | ウィンドウが開いている途中か |
| `_closing` | Boolean | ウィンドウが閉じている途中か |


### Extends

* [Window](Window.md)


### Inherited From

#### [PIXI.DisplayObject](PIXI.DisplayObject.md)

* [(static) mixin (source)](PIXI.DisplayObject.md#static-mixin-source)
* [\_recursivePostUpdateTransform ()](PIXI.DisplayObject.md#_recursivepostupdatetransform-)
* [displayObjectUpdateTransform ()](PIXI.DisplayObject.md#displayobjectupdatetransform-)
* [getBounds (skipUpdate, rect)](PIXI.DisplayObject.md#getbounds-skipupdate-rect--pixirectangle)
* [getGlobalPosition (point, skipUpdate)](PIXI.DisplayObject.md#getglobalposition-point-skipupdate--pixipoint)
* [setParent (container)](PIXI.DisplayObject.md#setparent-container--pixicontainer)
* [setTransform (x, y, scaleX, scaleY, rotation, skewX, skewY, pivotX, pivotY)](PIXI.DisplayObject.md#settransform-x-y-scalex-scaley-rotation-skewx-skewy-pivotx-pivoty--pixidisplayobject)
* [toGlobal (position, point, skipUpdate)](PIXI.DisplayObject.md#toglobal-position-point-skipupdate--pixipoint)
* [toLocal (position, from, point, skipUpdate)](PIXI.DisplayObject.md#tolocal-position-from-point-skipupdate--pixipoint)


#### [PIXI.Container](PIXI.Container.md)

* [addChild (child) ](PIXI.Container.md#addchild-child--pixidisplayobject)
* [addChildAt (child, index)](PIXI.Container.md#addchildat-child-index--pixidisplayobject)
* [calculateBounds ()](PIXI.Container.md#calculatebounds-)
* [destroy ()](PIXI.Container.md#destroy-)
* [getChildAt (index)](PIXI.Container.md#getchildat-index--pixidisplayobject)
* [getChildByName (name)](PIXI.Container.md#getchildbyname-name--pixidisplayobject)
* [getChildIndex (child)](PIXI.Container.md#getchildindex-child--pixidisplayobject)
* [onChildrenChange ()](PIXI.Container.md#onchildrenchange-)
* [removeChild (child)](PIXI.Container.md#removechild-child--pixidisplayobject)
* [removeChildAt (index)](PIXI.Container.md#removechildat-index--pixidisplayobject)
* [removeChildren (beginIndex, endIndex)](PIXI.Container.md#removechildren-beginindex-endindex--arraypixidisplayobject)
* [render (renderer)](PIXI.Container.md#render-renderer)
* [renderAdvanced (renderer)](PIXI.Container.md#renderadvanced-renderer)
* [renderCanvas (renderer)](PIXI.Container.md#rendercanvas-renderer)
* [setChildIndex (child, index)](PIXI.Container.md#setchildindex-child-index)
* [sortChildren ()](PIXI.Container.md#sortchildren-)
* [swapChildren (child, child2)](PIXI.Container.md#swapchildren-child-child2)

#### [Window](Window.md)

* [addChildToBack (child)](Window.md#addchildtoback-child--object)
* [isClosed ()](Window.md#isclosed---boolean)
* [isOpen ()](Window.md#isopen---boolean)
* [move (x, y, width, height)](Window.md#move-x-y-width-height)
* [setCursorRect (x, y, width, height)](Window.md#setcursorrect-x-y-width-height)
* [setTone (r, g, b)](Window.md#settone-r-g-b)
* [updateTransform ()](Window.md#updatetransform-)


### Methods

#### activate ()
ウィンドウをアクティブにする。


#### actorName (actorIndex) → {[String](String.md)}
指定された番号の[アクター]の名前を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actorIndex` | [Number](Number.md) | アクターの番号(1から始まる) |


#### calcTextHeight (textState, all) → {[Number](Number.md)}
指定したテキストの表示時の高さ(ピクセル)を計算して返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 計算するテキストの情報 |
| `all` | Boolean | 複数行を加算するか |


#### canvasToLocalX (x) → {[Number](Number.md)}
指定したCanvas の x座標を、ゲーム画面のローカルx座標に変換して返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | Canvas の x座標 |


#### canvasToLocalY (y) → {[Number](Number.md)}
指定したCanvas の y座標を、ゲーム画面のローカルy座標に変換して返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `y` | [Number](Number.md) | Canvas の y座標 |


#### changePaintOpacity (enabled)
背景を不透明にするか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `enabled` | Boolean | true: 不透明(255), false: 半透明(160) |


#### changeTextColor (color)
文字の色を設定。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `color` | [String](String.md) | 色(CSS形式) |


#### close ()
ウィンドウを閉じる。


#### contentsHeight () → {[Number](Number.md)}
ウィンドウに含まれるコンテンツの高さを返す。


#### contentsWidth () → {[Number](Number.md)}
ウィンドウに含まれるコンテンツの幅を返す。


#### convertEscapeCharacters (text) → {[String](String.md)}
エスケープ文字を変換して返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `text` | [String](String.md) | 変換元の文字列 |


#### createContents ()
テキストなどを表示するコンテンツ領域を生成。

#### crisisColor () → {[String](String.md)}
危険色(CSS形式)を返す。


#### deactivate ()
非アクティブにする。


#### deathColor () → {[String](String.md)}
死亡色(CSS形式)を返す。


#### dimColor1 () → {[String](String.md)}
Dimmer背景の色1(CSS形式)を返す。


#### dimColor2 () → {[String](String.md)}
Dimmer背景の色2(CSS形式)を返す。


#### drawActorCharacter (actor, x, y)
指定した[アクター]のキャラクタを指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### drawActorClass (actor, x, y, width)
指定した[アクター]の[クラス]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorFace (actor, x, y, width, height)
指定した[アクター]の顔画像を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |
| `height` | [Number](Number.md) | 描画領域の高さ(ピクセル) |


#### drawActorHp (actor, x, y, width)
指定した[アクター]の[HP]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorIcons (actor, x, y, width)
指定した[アクター]のアイコンを指定位置に描画。


##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorLevel (actor, x, y)
指定した[アクター]の[レベル]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### drawActorMp (actor, x, y, width)
指定した[アクター]の[MP]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorName (actor, x, y, width)
指定した[アクター]の[名前]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorNickname (actor, x, y, width)
指定した[アクター]の[二つ名]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorSimpleStatus (actor, x, y, width)
指定した[アクター]の簡易ステータスを指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawActorTp (actor, x, y, width)
指定した[アクター]の[TP]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawCharacter (characterName, characterIndex, x, y)
指定した'img/characters/'フォルダのファイル名とキャラクタ番号で、指定位置にキャラクタを描画。<br />
キャラクタ番号は左上から始まり右へ進み、2段目に移る。$付きの場合は0のみ。表示されるのは下向き中央のパターン。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `characterName` | [String](String.md) |  ファイル名(拡張子.pngを除く) |
| `characterIndex` | [Number](Number.md) | キャラクタ番号(0 〜 7)  |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### drawCurrencyValue (value, unit, x, y, width)
所持金を通貨単位付きで指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `value` | [Number](Number.md) | 所持金 |
| `unit` | [String](String.md) | 通貨単位 |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawCurrentAndMax (current, max, x, y, width, color1, color2)
現在値と最大値の組み合わせを指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `current` | [Number](Number.md) | 現在値 |
| `max` | [Number](Number.md) | 最大値 |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |
| `color1` | [String](String.md) | 現在値色(CSS形式) |
| `color2` | [String](String.md) | 最大値色(CSS形式) |


#### drawFace (faceName, faceIndex, x, y, width opt, height opt)
指定した'img/faces/'フォルダのファイル名とキャラクタ番号で、指定位置に顔画像を描画。<br />
キャラクタ番号は左上から始まり右へ進み、2段目に移る。

##### Parameters:

| Name | Type | Attributes | Description |
| --- | --- | --- | --- |
| `faceName` | [String](String.md) |  | ファイル名(拡張子.pngを除く) |
| `faceIndex` | [Number](Number.md) |  | キャラクタ番号(0 〜 7) |
| `x` | [Number](Number.md) |  | x座標(ピクセル) |
| `y` | [Number](Number.md) |  | y座標(ピクセル) |
| `width` | [Number](Number.md) | \<optional> | 幅(ピクセル) |
| `height` | [Number](Number.md) | \<optional> | 高さ(ピクセル) |


#### drawGauge (x, y, width, rate, color1, color2)
指定位置にゲージを描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 幅(ピクセル) |
| `rate` | [Number](Number.md) | 比率(0 〜 1) |
| `color1` | [String](String.md) | ゲージ色1(CSS形式) |
| `color2` | [String](String.md) | ゲージ色2(CSS形式) |


#### drawIcon (iconIndex, x, y)
指定した番号のアイコンを指定位置に描画。<br />
'img/system/IconSet.png'のファイルを16×20に分割した画像。
アイコン番号は左上から始まり右へ進み、端まで到達したら下へ進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `iconIndex` | [Number](Number.md) | アイコン番号(0 〜 319) |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### drawItemName (item, x, y, width)
指定した[アイテム]の[名前]を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `item` | [RPG.BaseItem](RPG.BaseItem.md) | 対象の[アイテム] |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |


#### drawText (text, x, y, maxWidth, align)
指定した文字列を指定位置に描画。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `text` |  [String](String.md) \| [Number](Number.md) | 表示する文字列 |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `maxWidth` | [Number](Number.md) | 最大許容幅(ピクセル) |
| `align` | [String](String.md) | 文字揃え(left, center, right) |


#### drawTextEx (text, x, y) → {[Number](Number.md)}
指定したエスケープ文字入の文字列を指定位置に描画し、x座標の差分を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `text` | [String](String.md) | 表示する文字列 |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### fittingHeight (numLines) → {[Number](Number.md)}
指定された行数に必要な高さを返す。<br />
高さ = 行数 * 行の高さ + パディング幅 * 2。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `numLines` | [Number](Number.md) | 行数 |


#### gaugeBackColor () → {[String](String.md)}
ゲージの背景色(CSS形式)を返す。


#### hide ()
ウィンドウを非表示(閉じるわけではない)。


#### hideBackgroundDimmer ()
Dimmer背景を非表示。


#### hpColor (actor) → {[String](String.md)}
指定した[アクター]の[HP]の色(CSS形式)を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |


#### hpGaugeColor1 () → {[String](String.md)}
[HP]ゲージの色1(CSS形式)を返す。


#### hpGaugeColor2 () → {[String](String.md)}
[HP]ゲージの色2(CSS形式)を返す。


#### initialize (x, y, width, height)
Overrides: [Window.initialize ()](Window.md#initialize-)

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `width` | [Number](Number.md) | 描画領域の幅(ピクセル) |
| `height` | [Number](Number.md) | 描画領域の高さ(ピクセル) |



#### isClosing () → {Boolean}
ウィンドウが閉じている途中か。


#### isOpening () → {Boolean}
ウィンドウが開いている途中か。


#### lineHeight () → {[Number](Number.md)}
行の高さ(ピクセル)を返す。規定値: 36


#### loadWindowskin ()
'img/system/Window.png'から、ウィンドウのスキンを読み込む。


#### makeFontBigger ()
フォントサイズを12大きくする。


#### makeFontSmaller ()
フォントサイズを12小さくする。


#### mpColor (actor) → {[String](String.md)}
指定した[アクター]の[MP]の色(CSS形式)を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |


#### mpCostColor () → {[String](String.md)}
[消費MP]の色(CSS形式)を返す。


#### mpGaugeColor1 () → {[String](String.md)}
[MP]ゲージの色1(CSS形式)を返す。


#### mpGaugeColor2 () → {[String](String.md)}
[MP]ゲージの色2(CSS形式)を返す。


#### normalColor () → {[String](String.md)}
通常色(CSS形式)を返す。


#### obtainEscapeCode (textState)
textStateのindex以降に含まれる制御文字本体を大文字で返す。<br />
indexは取り出した文字の数だけ進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### obtainEscapeParam (textState) → {Number|String}
textStateのindex以降に含まれる制御文字の添字を返す。<br />
indexは取り出した文字の数だけ進む。<br />
添字がある場合は数値が返り、ない場合は空文字が返る。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### open ()
ウィンドウを開く。


#### paramchangeTextColor (change) → {String}
指定した数値に対応する色(CSS形式)を返す。<br />
装備を変える際の能力差分の表示などに使う。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `change` | [Number](Number.md) | 負の値: powerDownColor, 0:normalColor, 正の値:powerUpColor |


#### partyMemberName (partyMemberIndex) → {[String](String.md)}
指定したパーティーメンバー番号に対応した名前を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `partyMemberIndex` | [Number](Number.md) | パーティーメンバー番号(1から開始される) |


#### pendingColor () → {[String](String.md)}
未決定色(CSS形式)を返す。


#### powerDownColor () → {[String](String.md)}
パワーダウン色(CSS形式)を返す。


#### powerUpColor () → {[String](String.md)}
パワーアップ色(CSS形式)を返す。


#### processCharacter (textState)
改行・改ページ・エスケープ文字などを含む文字を処理する。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### processDrawIcon (iconIndex, textState)
アイコン表示を処理。<br />
制御文字'\I[n]'の対応。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `iconIndex` | [Number](Number.md) | アイコン番号(0 〜 319) |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### processEscapeCharacter (code, textState)
制御文字の処理。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `code` | [String](String.md) | 制御文字(C I \{ \}) |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### processNewLine (textState)
改行の処理。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### processNewPage (textState)
改ページの処理。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### processNormalCharacter (textState)
通常文字の処理。<br />
処理した文字列の分だけindexは進む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `textState` | [MV.TextState](MV.TextState.md) | 処理する状態つき文字列 |


#### refreshDimmerBitmap ()
Dimmer背景を再描画。


#### reserveFaceImages ()
全パーティーメンバーの顔画像をキャッシュする。


#### resetFontSettings ()
フォント設定を規定値に戻す。


#### resetTextColor ()
文字色を規定値に戻す。


#### setBackgroundType (type)
背景の種類を設定。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `type` | [Number](Number.md) | 0:不透明度255 (標準), 1:薄暗く表示, その他:不透明度0 |


#### show ()
ウィンドウを表示。


#### showBackgroundDimmer ()
Dimmer背景を表示。


#### standardBackOpacity () → {[Number](Number.md)}
標準の背景の不透明度を返す。規定値:192


#### standardFontFace () → {[String](String.md)}
標準のフォント名を返す。


#### standardFontSize () → {[Number](Number.md)}
標準のフォントサイズを返す。規定値:28


#### standardPadding () → {[Number](Number.md)}
標準のパディング幅を返す。規定値:18


#### systemColor () → {[String](String.md)}
システム色(CSS形式)を返す。


#### textColor (n) → {[String](String.md)}
指定した番号に対応する色(CSS形式)を返す。<br />
'img/system/window.png' の色で設定される。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `n` | [Number](Number.md) | カラー番号(0 〜 31) |


#### textPadding () → {[Number](Number.md)}
パディング幅を返す。規定値:6


#### textWidth (text) → {[Number](Number.md)}
指定文字列の幅(ピクセル)を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `text` | [String](String.md) | 測定する文字列 |


#### tpColor (actor) → {[String](String.md)}
指定した[アクター]の[TP]の色(CSS形式)を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | 対象の[アクター] |


#### tpCostColor () → {[String](String.md)}
[消費TP]の色(CSS形式)を返す。


#### tpGaugeColor1 () → {[String](String.md)}
[TP]ゲージの色1(CSS形式)を返す。


#### tpGaugeColor2 () → {[String](String.md)}
[TP]ゲージの色2(CSS形式)を返す。


#### translucentOpacity () → {[Number](Number.md)}
ウィンドウ背景の不透明度を返す。規定値:160


#### update ()
Overrides: [Window.update ()](Window#update-)


#### updateBackgroundDimmer ()
Dimmer背景のアップデート。


#### updateBackOpacity ()
背景の不透明度をアップデート。


#### updateClose ()
ウィンドウを閉じている状態をアップデート。


#### updateOpen ()
ウィンドウを開いている状態をアップデート。


#### updatePadding ()
パディング幅をアップデート。


#### updateTone ()
色調をアップデート。


 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
