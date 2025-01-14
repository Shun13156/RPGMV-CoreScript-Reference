# Class: Window_EquipStatus

## Window_EquipStatus (x, y)

#### new Window_EquipStatus (x, y)

装備時のパラメータの変化を表示するウィンドウ。


##### Parameters:

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |

##### Properties:

| Parameter | Type | Description |
| --- | --- | --- |
| `_actor` | [Game_Actor](Game_Actor.md) | アクター |
| `_tempActor` | [Game_Actor](Game_Actor.md) | 作業用のアクター |


### Extends

* [Window_Base](Window_Base.md)


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

#### [Window_Base](Window_Base.md)
* [activate ()](Window_Base.md#activate-)* [actorName (actorIndex)](Window_Base.md#actorname-actorindex--string)* [calcTextHeight (textState, all)](Window_Base.md#calctextheight-textstate-all--number)* [canvasToLocalX (x)](Window_Base.md#canvastolocalx-x--number)* [canvasToLocalY (y)](Window_Base.md#canvastolocaly-y--number)* [changePaintOpacity (enabled)](Window_Base.md#changepaintopacity-enabled)* [changeTextColor (color)](Window_Base.md#changetextcolor-color)* [close ()](Window_Base.md#close-)* [contentsWidth ()](Window_Base.md#contentswidth---number)* [convertEscapeCharacters (text)](Window_Base.md#convertescapecharacters-text--string)* [createContents ()](Window_Base.md#createcontents-)* [crisisColor ()](Window_Base.md#crisiscolor---string)* [deactivate ()](Window_Base.md#deactivate-)* [deathColor ()](Window_Base.md#deathcolor---string)* [dimColor1 ()](Window_Base.md#dimcolor1---string)* [dimColor2 ()](Window_Base.md#dimcolor2---string)* [drawActorCharacter (actor, x, y)](Window_Base.md#drawactorcharacter-actor-x-y)* [drawActorClass (actor, x, y, width)](Window_Base.md#drawactorclass-actor-x-y-width)* [drawActorFace (actor, x, y, width, height)](Window_Base.md#drawactorface-actor-x-y-width-height)* [drawActorHp (actor, x, y, width)](Window_Base.md#drawactorhp-actor-x-y-width)* [drawActorIcons (actor, x, y, width)](Window_Base.md#drawactoricons-actor-x-y-width)* [drawActorLevel (actor, x, y)](Window_Base.md#drawactorlevel-actor-x-y)* [drawActorMp (actor, x, y, width)](Window_Base.md#drawactormp-actor-x-y-width)* [drawActorName (actor, x, y, width)](Window_Base.md#drawactorname-actor-x-y-width)* [drawActorNickname (actor, x, y, width)](Window_Base.md#drawactornickname-actor-x-y-width)* [drawActorSimpleStatus (actor, x, y, width)](Window_Base.md#drawactorsimplestatus-actor-x-y-width)* [drawActorTp (actor, x, y, width)](Window_Base.md#drawactortp-actor-x-y-width)* [drawCharacter (characterName, characterIndex, x, y)](Window_Base.md#drawcharacter-charactername-characterindex-x-y)* [drawCurrencyValue (value, unit, x, y, width)](Window_Base.md#drawcurrencyvalue-value-unit-x-y-width)* [drawCurrentAndMax (current, max, x, y, width, color1, color2)](Window_Base.md#md#drawcurrentandmax-current-max-x-y-width-color1-color2)* [drawFace (faceName, faceIndex, x, y, width opt, height opt)](Window_Base.md#drawface-facename-faceindex-x-y-width-opt-height-opt)* [drawGauge (x, y, width, rate, color1, color2)](Window_Base.md#drawgauge-x-y-width-rate-color1-color2)* [drawIcon (iconIndex, x, y)](Window_Base.md#drawicon-iconindex-x-y)* [drawItemName (item, x, y, width)](Window_Base.md#drawitemname-item-x-y-width)* [drawText (text, x, y, maxWidth, align)](Window_Base.md#drawtext-text-x-y-maxwidth-align)* [drawTextEx (text, x, y)](Window_Base.md#drawtextex-text-x-y--number)* [fittingHeight (numLines)](Window_Base.md#fittingheight-numlines--number)* [gaugeBackColor ()](Window_Base.md#gaugebackcolor---string)* [hide ()](Window_Base.md#hide-)* [hideBackgroundDimmer ()](Window_Base.md#hidebackgrounddimmer-)* [hpColor (actor)](Window_Base.md#hpcolor-actor--string)* [hpGaugeColor1 ()](Window_Base.md#hpgaugecolor1---string)* [hpGaugeColor2 ()](Window_Base.md#hpgaugecolor2---string)* [isClosing ()](Window_Base.md#isclosing---boolean)* [isOpening ()](Window_Base.md#isopening---boolean)* [lineHeight ()](Window_Base.md#lineheight---number)* [loadWindowskin ()](Window_Base.md#loadwindowskin-)* [makeFontBigger ()](Window_Base.md#makefontbigger-)* [makeFontSmaller ()](Window_Base.md#makefontsmaller-)* [mpColor (actor)](Window_Base.md#mpcolor-actor--string)* [mpCostColor ()](Window_Base.md#mpcostcolor---string)* [mpGaugeColor1 ()](Window_Base.md#mpgaugecolor1---string)* [mpGaugeColor2 ()](Window_Base.md#mpgaugecolor2---string)* [normalColor ()](Window_Base.md#normalcolor---string)* [obtainEscapeCode (textState)](Window_Base.md#obtainescapecode-textstate)* [obtainEscapeParam (textState)](Window_Base.md#obtainescapeparam-textstate--numberstring)* [open ()](Window_Base.md#open-)* [paramchangeTextColor (change)](Window_Base.md#paramchangetextcolor-change--string)* [partyMemberName (partyMemberIndex)](Window_Base.md#partymembername-partymemberindex--string)* [pendingColor ()](Window_Base.md#pendingcolor---string)* [powerDownColor ()](Window_Base.md#powerdowncolor---string)* [powerUpColor ()](Window_Base.md#powerupcolor---string)* [processCharacter (textState)](Window_Base.md#processcharacter-textstate)* [processDrawIcon (iconIndex, textState)](Window_Base.md#processdrawicon-iconindex-textstate)* [processEscapeCharacter (code, textState)](Window_Base.md#processescapecharacter-code-textstate)* [processNewLine (textState)](Window_Base.md#processnewline-textstate)* [processNewPage (textState)](Window_Base.md#processnewpage-textstate)* [processNormalCharacter (textState)](Window_Base.md#processnormalcharacter-textstate)* [refreshDimmerBitmap ()](Window_Base.md#refreshdimmerbitmap-)* [reserveFaceImages ()](Window_Base.md#reservefaceimages-)* [resetFontSettings ()](Window_Base.md#resetfontsettings-)* [resetTextColor ()](Window_Base.md#resettextcolor-)* [setBackgroundType (type)](Window_Base.md#setbackgroundtype-type)* [show ()](Window_Base.md#show-)* [showBackgroundDimmer ()](Window_Base.md#showbackgrounddimmer-)* [standardBackOpacity ()](Window_Base.md#standardbackopacity---number)* [standardFontFace ()](Window_Base.md#standardfontface---string)* [standardFontSize ()](Window_Base.md#standardfontsize---number)* [standardPadding ()](Window_Base.md#standardpadding---number)* [systemColor ()](Window_Base.md#systemcolor---string)* [textColor (n)](Window_Base.md#textcolor-n--string)* [textPadding ()](Window_Base.md#textpadding---number)* [textWidth (text)](Window_Base.md#textwidth-text--number)* [tpColor (actor)](Window_Base.md#tpcolor-actor--string)* [tpCostColor ()](Window_Base.md#tpcostcolor---string)* [tpGaugeColor1 ()](Window_Base.md#tpgaugecolor1---string)* [tpGaugeColor2 ()](Window_Base.md#tpgaugecolor2---string)* [translucentOpacity ()](Window_Base.md#translucentopacity---number)* [update ()](Window_Base.md#update-)* [updateBackgroundDimmer ()](Window_Base.md#updatebackgrounddimmer-)* [updateBackOpacity ()](Window_Base.md#updatebackopacity-)* [updateClose ()](Window_Base.md#updateclose-)* [updateOpen ()](Window_Base.md#updateopen-)* [updatePadding ()](Window_Base.md#updatepadding-)* [updateTone ()](Window_Base.md#updatetone-)

### Methods

#### drawCurrentParam (x, y, paramId)
現在のパラメータを描く。

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `paramId` | [Number](Number.md) | パラメータのID |



#### drawItem (x, y, paramId)
アイテムを描く。

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `paramId` | [Number](Number.md) | パラメータのID |


#### drawNewParam (x, y, paramId)
装備後のパラメータを描く。

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `paramId` | [Number](Number.md) | パラメータのID |


#### drawParamName (x, y, paramId)
パラメータの名前を描く。

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `paramId` | [Number](Number.md) | パラメータのID |


#### drawRightArrow (x, y)
矢印(→)を描く。

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### initialize (x, y)
Overrides: [Window_Base.initialize (x, y, width, height)](Window_Base.md#initialize-x-y-width-height)

| Parameter | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |


#### numVisibleRows () → {[Number](Number.md)}
表示されている行の数を返す。


#### refresh ()
再描画。


#### setActor (actor)
対象となるアクターを設定。

| Parameter | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | アクター |


#### setTempActor (actor)
作業対象となるアクターを設定。

| Parameter | Type | Description |
| --- | --- | --- |
| `actor` | [Game_Actor](Game_Actor.md) | アクター |


#### windowHeight () → {[Number](Number.md)}
ウィンドウの高さ(ピクセル)を返す。


#### windowWidth () → {[Number](Number.md)}
ウィンドウの幅(ピクセル)を返す。