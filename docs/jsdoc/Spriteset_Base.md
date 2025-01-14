# Class: Spriteset_Base

## (abstract) Spriteset_Base ()

#### (abstract) new Spriteset_Base ()

複数のスプライトを組み合わせて使うクラス。

[Spriteset_Map](Spriteset_Map.md) と [Spriteset_Battle](Spriteset_Battle.md) のスーパークラス。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `_tone` | [Array](Array.md).&lt;[Number](Number.md)&gt; | 色調 |
| `_baseSprite` | [Sprite](Sprite.md) | 基本スプライト |
| `_blackScreen` | [ScreenSprite](ScreenSprite.md) |  |
| `_toneFilter` | [ToneFilter](ToneFilter.md) |  |
| `_toneSprite` | [ToneSprite](ToneSprite.md) |  |
| `_pictureContainer` | [Sprite](Sprite.md) |  |
| `_timerSprite` | [Sprite_Timer](Sprite_Timer.md) |  |
| `_flashSprite` | [ScreenSprite](ScreenSprite.md) |  |
| `_fadeSprite` | [ScreenSprite](ScreenSprite.md) |  |


### Extends

* [Sprite](Sprite.md)


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
* [getChildAt (index)](PIXI.Container.md#getchildat-index--pixidisplayobject)
* [getChildByName (name)](PIXI.Container.md#getchildbyname-name--pixidisplayobject)
* [getChildIndex (child)](PIXI.Container.md#getchildindex-child--pixidisplayobject)
* [onChildrenChange ()](PIXI.Container.md#onchildrenchange-)
* [removeChild (child)](PIXI.Container.md#removechild-child--pixidisplayobject)
* [removeChildAt (index)](PIXI.Container.md#removechildat-index--pixidisplayobject)
* [removeChildren (beginIndex, endIndex)](PIXI.Container.md#removechildren-beginindex-endindex--arraypixidisplayobject)
* [render (renderer)](PIXI.Container.md#render-renderer)
* [renderAdvanced (renderer)](PIXI.Container.md#renderadvanced-renderer)
* [setChildIndex (child, index)](PIXI.Container.md#setchildindex-child-index)
* [sortChildren ()](PIXI.Container.md#sortchildren-)
* [swapChildren (child, child2)](PIXI.Container.md#swapchildren-child-child2)
* [updateTransform ()](PIXI.Container.md#updatetransform-)


#### [PIXI.Sprite](PIXI.Sprite.md)

* [(static) from (source, options)](PIXI.Sprite.md#static-from-source-options--pixisprite)
* [\_calculateBounds ()](PIXI.Sprite.md#_calculatebounds-)
* [\_render (renderer)](PIXI.Sprite.md#_render-renderer)
* [calculateTrimmedVertices ()](PIXI.Sprite.md#calculatetrimmedvertices-)
* [calculateVertices ()](PIXI.Sprite.md#calculatevertices-)
* [containsPoint (point)](PIXI.Sprite.md#containspoint-point--boolean)
* [destroy (options)](PIXI.Sprite.md#destroy-options)
* [getLocalBounds (rect)](PIXI.Sprite.md#getlocalbounds-rect--pixirectangle)
* [renderCanvas (renderer)](PIXI.Sprite.md#rendercanvas-renderer)


#### [Sprite](Sprite.md)

* [\_createTinter (w, h)](Sprite.md#_createtinter-w-h)
* [\_executeTint (x, y, w, h)](Sprite.md#_executetint-x-y-w-h)
* [\_isInBitmapRect (x, y, w, h)](Sprite.md#_isinbitmaprect-x-y-w-h--boolean)
* [\_needsTint ()](Sprite.md#_needstint---boolean)
* [\_onBitmapLoad ()](Sprite.md#_onbitmapload-)
* [\_refresh ()](Sprite.md#_refresh-)
* [\_renderCanvas (renderer)](Sprite.md#_rendercanvas-renderer)
* [\_renderWebGL (renderer)](Sprite.md#_renderwebgl-renderer)
* [\_speedUpCustomBlendModes (renderer)](Sprite.md#_speedupcustomblendmodes-renderer)
* [getBlendColor ()](Sprite.md#getblendcolor---array)
* [getColorTone ()](Sprite.md#getcolortone---array)
* [move (x, y)](Sprite.md#Sprite.md#move-x-y)
* [setBlendColor (color)](Sprite.md#setblendcolor-color)
* [setColorTone (tone)](Sprite.md#setcolortone-tone)
* [setFrame (x, y, width, height)](Sprite.md#setframe-x-y-width-height)


### Methods

#### createBaseSprite ()
 基本スプライトを生成。


#### createCanvasToneChanger ()
canvas 色調変更を生成。


#### createLowerLayer ()
 基本スプライトを含む下レイヤを生成。


#### createPictures ()
 画像スプライトを生成。


#### createScreenSprites ()
 画面スプライトを生成。


#### createTimer ()
 タイマースプライトを生成。


#### createToneChanger ()
 色調補正スプライトを生成。


#### createUpperLayer ()
 画像, タイマー, スクリーンスプライトを含む上レイヤを生成。


#### createWebGLToneChanger ()
WebGL 色調変更を生成。


#### initialize ()
 オブジェクト生成時の初期化。
 
##### Overrides
[Sprite.initialize()](Sprite.md#initialize-)


#### update ()
フレーム毎のアップデート。

##### Overrides
[Sprite.update()](Sprite.md#update-)


#### updateCanvasToneChanger ()
canvas 色調変更をアップデート。


#### updatePosition ()
 位置をアップデート。


#### updateScreenSprites ()
 画面スプライトをアップデート。


#### updateToneChanger ()
 色調変更をアップデート。


#### updateWebGLToneChanger ()
WebGL 色調変更をアップデート。



 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
