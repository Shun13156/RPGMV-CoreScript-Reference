# Class: PIXI.DisplayObject

## PIXI.DisplayObject ()

#### new PIXI.DisplayObject ()

画面に表示されるもの一般の基本となるオブジェクト。

[PIXI.Container](PIXI.Container.md) のスーパークラス。

詳細は本家 PIXI のサイト [PIXI.DisplayObject](http://pixijs.download/release/docs/PIXI.DisplayObject.html) を参照。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `_accessibleDiv` | Boolean |  |
| `_bounds` | [PIXI.Bounds](http://pixijs.download/release/docs/PIXI.Bounds.html) | 矩形範囲 |
| `_destroyed` | Boolean | destroy() により破棄されているか |
| `_lastSortedIndex` | [Number](Number.md) | 最終ソート番号 |
| `_mask` | [PIXI.Graphics](http://pixijs.download/release/docs/PIXI.Graphics.html) \| [PIXI.Sprite](PIXI.Sprite.md) \| null | マスク画像 |
| `_tempDisplayObjectParent` | PIXI.DisplayObject | 仮の親オブジェクト |
| `_zIndex` | [Number](Number.md) | 高い番号ほど手前に表示される番号 |
| `accessible` | Boolean | 操作可能か |
| `accessibleHint` | [String](String.md) |  |
| `accessibleTitle` | [String](String.md) |  |
| `alpha` | [Number](Number.md) | 不透明度 |
| `angle` | [Number](Number.md) | 回転角(角度) |
| `buttonMode` | Boolean | マウスオーバー時などポインタが変更されるか |
| `cacheAsBitmap` | Boolean |ビットマップとしてキャッシュされるか |
| `cursor` | [String](String.md) | マウスオーバー時のポインタの種類 |
| `filterArea` | [PIXI.Rectangle](http://pixijs.download/release/docs/PIXI.Rectangle.html) | フィルタ範囲 |
| `filters` | [Array](Array.md).&lt;[PIXI.Filter](http://pixijs.download/dev/docs/PIXI.Filter.html)&gt; | フィルタの配列 |
| `hitArea` | [PIXI.IHitArea](http://pixijs.download/release/docs/PIXI.IHitArea.html) | (クリック)判定範囲 |
| `interactive` | Boolean | (クリック)操作可能か |
| `isSprite` | Boolean | スプライトか |
| `localTransform` | [PIXI.Matrix](http://pixijs.download/release/docs/PIXI.Matrix.html) | [read-only]ローカルな変形 |
| `mask` | [PIXI.Graphics](http://pixijs.download/release/docs/PIXI.Graphics.html) \| [PIXI.Sprite](PIXI.Sprite.md) \| null | マスク画像 |
| `name` | [String](String.md) | 名前 |
| `parent` | [PIXI.Container](http://pixijs.download/dev/docs/PIXI.Container.html) | [read-only] 親コンテナオブジェクト |
| `pivot` | [PIXI.IPoin](http://pixijs.download/release/docs/PIXI.html#.IPoint) | 回転軸 |
| `position` | [Point](Point.md) | 位置(x, y を同時に指定) |
| `renderable` | Boolean | レンダ可能か |
| `rotation` | [Number](Number.md) | 回転角(ラジアン) |
| `scale` | [PIXI.IPoin](http://pixijs.download/release/docs/PIXI.html#.IPoint) | 拡大率 |
| `skew` | [PIXI.ObservablePoint](http://pixijs.download/release/docs/PIXI.ObservablePoint.html) | 傾斜 |
| `transform` | [PIXI.Matrix](http://pixijs.download/release/docs/PIXI.Matrix.html) | 変形 |
| `visible` | Boolean |  表示中か |
| `worldAlpha` | [Number](Number.md) | [read-only] 最終的な不透明度 |
| `worldTransform` | [PIXI.Matrix](http://pixijs.download/release/docs/PIXI.Matrix.html) | [read-only] 最終的な変形 |
| `worldVisible` | Boolean |  [read-only] 最終的に表示中か |
| `x` | [Number](Number.md) | x座標(ピクセル) |
| `y` | [Number](Number.md) | y座標(ピクセル) |
| `zIndex` | [Number](Number.md) | 高い番号ほど手前に表示される番号 |


### Extends

* [PIXI.utils.EventEmitter](http://pixijs.download/release/docs/PIXI.utils.EventEmitter.html)

### Methods

#### (static) mixin (source)
指定オブジェクトを元に、列挙可能なすべてのプロパティとメソッドをミックスインさせます。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `source` | Object | ミックスインの元となるオブジェクト |


#### _recursivePostUpdateTransform ()


#### destroy ()
破棄する。


#### displayObjectUpdateTransform ()


#### getBounds (skipUpdate, rect) → {PIXI.Rectangle}
矩形範囲を得る。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `skipUpdate` | Boolean | opt. |
| `rect` | PIXI.Rectangle | opt. |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Rectangle.html">PIXI.Rectangle</a></span>
    </dd>
</dl>


#### getGlobalPosition (point, skipUpdate) → {PIXI.Point}


##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `point` | PIXI.Point | opt. |
| `skipUpdate` | Boolean | opt. |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Rectangle.html">PIXI.Point</a></span>
    </dd>
</dl>


#### getLocalBounds (rect) → {PIXI.Rectangle}

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `rect` | PIXI.Rectangle | opt. |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Rectangle.html">PIXI.Rectangle</a></span>
    </dd>
</dl>


#### render (renderer)

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `renderer` | [PIXI.Renderer](http://pixijs.download/release/docs/PIXI.Renderer.html) |  |


#### setParent (container) → {PIXI.Container}
親オブジェクトを設定。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `container ` | PIXI.Container | 親に指定するコンテナオブジェクト |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Container.html"> PIXI.Container </a></span>
    </dd>
</dl>


#### setTransform (x, y, scaleX, scaleY, rotation, skewX, skewY, pivotX, pivotY) → {PIXI.DisplayObject}
まとめて変形を設定する。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x座標 |
| `y` | [Number](Number.md) | y座標 |
| `scaleX` | [Number](Number.md) | x拡大率 |
| `scaleY` | [Number](Number.md) | y拡大率 |
| `rotation` | [Number](Number.md) | 回転角(ラジアン) |
| `skewX` | [Number](Number.md) | x傾斜 |
| `skewY` | [Number](Number.md) | y傾斜 |
| `pivotX` | [Number](Number.md) | 回転軸x座標 |
| `pivotY` | [Number](Number.md) | 回転軸y座標 |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="PIXI.DisplayObject.html">PIXI.DisplayObject </a></span>
    </dd>
</dl>


#### toGlobal (position, point, skipUpdate) → {PIXI.Point}
グローバル座標に変換。

##### Parameters:

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| `position` |  | PIXI.Point | 変換元の座標 |
| `point` |  | PIXI.Point | opt. |
| `skipUpdate` | false | Boolean | opt. |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Rectangle.html">PIXI.Point</a></span>
    </dd>
</dl>


#### toLocal (position, from, point, skipUpdate) → {PIXI.Point}
ローカル座標に変換。

##### Parameters:

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| `position` |  | PIXI.Point | 変換元の座標 |
| `from` |  | PIXI.DisplayObject | opt. |
| `point` |  | PIXI.Point | opt. |
| `skipUpdate` | false | Boolean | opt. |

##### Returns:

<dl>
    <dt> Type </dt>
    <dd>
        <span><a href="http://pixijs.download/release/docs/PIXI.Rectangle.html">PIXI.Point</a></span>
    </dd>
</dl>


#### updateTransform ()
 変形のアップデート。


### Events

#### added(container)

| Name | Type | Description |
| --- | --- | --- |
| `container` | [PIXI.Container](PIXI.Container.md) | 子が追加されたコンテナ |


#### click(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mousedown(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mousemove(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mouseout(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mouseover(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mouseup(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### mouseupoutside(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointercancel(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointerdown(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointermove(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointerout(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointerover(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointertap(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointerup(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### pointerupoutside(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### removed(container)

| Name | Type | Description |
| --- | --- | --- |
| `container` | [PIXI.Container](PIXI.Container.md) | 子が削除されたコンテナ |

#### rightclick(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### rightdown(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### rightup(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### rightupoutside(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### tap(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### touchcancel(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### touchend(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### touchendoutside(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### touchmove(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


#### touchstart(event)

| Name | Type | Description |
| --- | --- | --- |
| `event` | [PIXI.interaction.InteractionEvent](http://pixijs.download/release/docs/PIXI.interaction.InteractionEvent.html) | 操作イベント |


 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
