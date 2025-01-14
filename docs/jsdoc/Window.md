# Class: Window

## Window ()

#### new Window ()

ゲーム内で使われるウィンドウ。[Window_Base](Window_Base.md)のスーパークラス。

ブラウザやその他アプリケーションのウィンドウではない。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `children` | [Array](Array.md).&lt;\*&gt; | [super][read-only] 子オブジェクト |
| `parent` | [PIXI.Container](http://pixijs.download/release/docs/PIXI.Container.html) | [super][read-only] 親オブジェクト |
| `active` | Boolean | ウィンドウがアクティブか |
| `openness` | [Number](Number.md) | 開放度 (0 〜 255) |
| `contents` | [Bitmap](Bitmap.md) | コンテンツ |
| `windowskin` | [Bitmap](Bitmap.md) | ウィンドウのスキンに使う画像 |
| `visible` | Boolean | ウィンドウが表示中か |
| `pause` | Boolean | ポーズサインが表示中か |
| `downArrowVisible` | Boolean | 下向きスクロールアローが表示中か|
| `upArrowVisible` | Boolean | 上むきスクロールアローが表示中か |
| `opacity` | [Number](Number.md) | コンテンツの不透明度(0 〜 255) |
| `backOpacity` | [Number](Number.md) | 背景の不透明度(0 〜 255) |
| `contentsOpacity` | [Number](Number.md) | コンテンツの不透明度(0 〜 255) |
| `origin` | [Point](Point.md) | スクロールの際のウィンドウの原点 |
| `x` | [Number](Number.md) | ウィンドウ x座標(ピクセル) |
| `y` | [Number](Number.md) | ウィンドウ y座標(ピクセル) |
| `width` | [Number](Number.md) | 拡大縮小前のウィンドウ幅(ピクセル) |
| `height` | [Number](Number.md) | 拡大縮小前のウィンドウ高さ(ピクセル) |
| `margin` | [Number](Number.md) | 背景マージン幅(ピクセル) |
| `padding` | [Number](Number.md) | 枠とコンテンツの間のパディング幅(ピクセル) |
| `_isWindow` | Boolean | ウィンドウか |
| `_windowskin` | [Bitmap](Bitmap.md) | ウィンドウのスキンに使う画像 |
| `_width` | [Number](Number.md) | 幅 |
| `_height` | [Number](Number.md) | 高さ |
| `_cursorRect` | [Rectangle](Rectangle.md) | カーソル矩形 |
| `_openness` | [Number](Number.md) | 開放度  |
| `_animationCount` | [Number](Number.md) | アニメーションカウント |
| `_padding` | [Number](Number.md) | パディング |
| `_margin` | [Number](Number.md) | マージン |
| `_colorTone` | [Array](Array.md).&lt;[Number](Number.md)&gt; | 色調 |
| `_windowSpriteContainer` | [PIXI.Container](http://pixijs.download/release/docs/PIXI.Container.html) | 画像コンテナ |
| `_windowBackSprite` | [Sprite](Sprite.md) | 背景 |
| `_windowCursorSprite` | [Sprite](Sprite.md) | カーソル |
| `_windowFrameSprite` | [Sprite](Sprite.md) | 枠 |
| `_windowContentsSprite` | [Sprite](Sprite.md) | 内容 |
| `_windowArrowSprites` | [Array](Array.md).&lt;\*&gt; | 矢印 |
| `_windowPauseSignSprite` | [Sprite](Sprite.md) | ポーズサイン |
| `_downArrowSprite` | [Sprite](Sprite.md) | 下向き矢印 |
| `_upArrowSprite` | [Sprite](Sprite.md) | 上向き矢印 |


### Extends

* [PIXI.Container](PIXI.Container.md)


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


### Methods

####  _createAllParts ()
ウィンドウの表示に必要な部品を生成する。

####  _onWindowskinLoad ()
スキンがダウンロードされたときのハンドラ。

####  _refreshAllParts ()
部品の再描画。

####  _refreshArrows ()
矢印の再描画。

####  _refreshBack ()
背景の再描画。

####  _refreshContents ()
内容の再描画。

####  _refreshCursor ()
カーソルの再描画。

####  _refreshFrame ()
枠の再描画。

####  _refreshPauseSign ()
ポーズサインの再描画。

####  _updateArrows ()
矢印のアップデート。

####  _updateContents ()
内容のアップデート。

####  _updateCursor ()
カーソルのアップデート。

####  _updatePauseSign ()
ポーズサインのアップデート。

#### addChildToBack (child) → {Object}
背景とコンテンツの間に子オブジェクトを追加し、追加されたオブジェクトを返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `child` | [PIXI.DisplayObject](PIXI.DisplayObject.md)  | 追加するオブジェクト |


#### initialize ()
 オブジェクト生成時の初期化。


#### isClosed () → {Boolean}
ウィンドウが完全に閉じているか。<br />
つまり、openness === 0 であるか。


#### isOpen () → {Boolean}

ウィンドウが完全に開いているか。<br />
つまり、openness === 255 であるか。


#### move (x, y, width, height)
指定した位置と大きさにウィンドウを変更。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | ウィンドウ x座標(ピクセル) |
| `y` | [Number](Number.md) | ウィンドウ y座標(ピクセル) |
| `width` | [Number](Number.md) | ウィンドウ幅(ピクセル) |
| `height` | [Number](Number.md) | ウィンドウ高さ(ピクセル) |


#### setCursorRect (x, y, width, height)
コマンド用カーソルの位置と大きさを設定。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | カーソル x座標(ピクセル) |
| `y` | [Number](Number.md) | カーソル y座標(ピクセル) |
| `width` | [Number](Number.md) | カーソル幅(ピクセル) |
| `height` | [Number](Number.md) | カーソル高さ(ピクセル) |


#### setTone (r, g, b)
背景の色調を設定。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `r` | [Number](Number.md) | 赤(-255 〜 255) |
| `g` | [Number](Number.md) | 緑(-255 〜 255) |
| `b` | [Number](Number.md) | 青(-255 〜 255) |


#### update ()
フレーム毎のアップデート。


#### updateTransform ()
Overrides: [PIXI.Container.updateTransform ()](PIXI.Container.md#updatetransform-)


 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
