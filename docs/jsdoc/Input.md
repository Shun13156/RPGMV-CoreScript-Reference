# Class: Input

キーボードとゲームパッド(コントローラ)の入力に関する静的クラス。<br />
JavaScriptの[KeyboardEvent](https://developer.mozilla.org/ja/docs/Web/API/KeyboardEvent)と[Gamepad](https://developer.mozilla.org/en-US/docs/Web/API/Gamepad)周りを扱う。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `keyRepeatWait` | [Number](Number.md) | [static] キーリピートまでの待ち時間(フレーム) |
| `keyRepeatInterval` | [Number](Number.md) | [static] キーリピート間隔(フレーム) |
| `keyMapper` | Object | [static] キーコードとキー名称の変換テーブル<br/> { code: 'name', ...} |
| `gamepadMapper` | Object | [static] ゲームパッドのボタンとキー名称の変換テーブル |
| `dir4` | [Number](Number.md) | [static][read-only] 4方向入力の数値( 0 : ニュートラル 他はテンキー方向) |
| `dir8` | [Number](Number.md) | [static][read-only]  8方向入力の数値( 0 : ニュートラル 他はテンキー方向) |
| `date` | [Number](Number.md) | [static][read-only] 最後に入力された時刻(ミリ秒) |
| `_currentState` | Object | [static] 現在の入力状態 {[key: string]: boolean} |
| `_previousState` | Object | [static] 直前の入力状態 {[key: string]: boolean} |
| `_gamepadStates` | [Array](Array.md).\<[Array](Array.md).\<Boolean\>\> | [static] ゲームパッドの状態 |
| `_latestButton` | [String](String.md) | [static] 最新のボタン |
| `_pressedTime` | [Number](Number.md) | [static] 入力時間 |
| `_dir4` | [Number](Number.md) | [static] 4方向入力の数値(通常dir4を使う) |
| `_dir8` | [Number](Number.md) | [static] 8方向入力の数値(通常dir8を使う) |
| `_preferredAxis` | [String](String.md) | [static] xとyのうち優先軸(4方向入力を自然にするのに使われる)|
| `_date` | [Number](Number.md) | [static] 入力時刻(通常dateを使う) |


### Methods

#### (static) _isEscapeCompatible (keyName) → {Boolean}
ESCキーに当たるキー(cancel, menu)か

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyName` | [String](String.md) | キー名称 |


##### Returns:

<dl>
	<dt> Type </dt>
	<dd>
		<span>Boolean</span>
	</dd>
</dl>

#### (static) _makeNumpadDirection (x, y) → {[Number](Number.md)}

x,y方向の入力からテンキー方向を生成

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `x` | [Number](Number.md) | x方向の入力(-1, 0, 1) |
| `y` | [Number](Number.md) | y方向の入力(-1, 0, 1) |


##### Returns:
入力のテンキー方向のでの表現(0 : ニュートラル)
<dl>
	<dt> Type </dt>
	<dd>
		<span>Number</span>
	</dd>
</dl>

#### (static) _onKeyDown (event)
キーが押し下げられた時に呼ばれるイベントハンドラ

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `event` | KeyboardEvent | キーボードイベント |


#### (static) _onKeyUp (event)
キーが離された時に呼ばれるイベントハンドラ

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `event` | KeyboardEvent | キーボードイベント |


#### (static) _onLostFocus ()
フォーカスが外れた時に呼ばれるイベントハンドラ

#### (static) _pollGamepads ()
ゲームパッドの状態を監視(ポーリング)する関数

#### (static) _setupEventHandlers ()
イベントハンドラの設定

#### (static) _shouldPreventDefault (keyCode)
イベントの規定動作を防ぐか。<br/>
keyCode が 33:pageup, 34:pagedown, 37:left, 38:up, 39:right, 40:down のいずれかであった場合 true を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyCode` | [Number](Number.md) | キーコード |

##### Returns:

* Boolean

#### (static) _signX ()
x軸の入力

##### Returns:
-1, 0, 1 のいずれかの値

* Number

#### (static) _signY ()
y軸の入力

##### Returns:
-1, 0, 1 のいずれかの値

* Number


#### (static) _updateDirection ()

向きをアップデート

#### (static) _updateGamepadState (gamepad, index)

ゲームパッドの状態をアップデート

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `gamepad` | Gamepad | ゲームパッドオブジェクト |

#### (static) _wrapNwjsAlert ()
NW.jsの警告のラッパ

#### (static) clear ()

入力データを初期化

#### (static) initialize ()

Inputオブジェクトの初期化

#### (static) isLongPressed (keyName) → {Boolean}

長押し状態か

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyName` | [String](String.md) | キー名称 |


##### Returns:

<dl>
	<dt> Type </dt>
	<dd>
		<span>Boolean</span>
	</dd>
</dl>

#### (static) isPressed (keyName) → {Boolean}

押されているか


##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyName` | [String](String.md) | キー名称 |


##### Returns:

<dl>
	<dt> Type </dt>
	<dd>
		<span>Boolean</span>
	</dd>
</dl>

#### (static) isRepeated (keyName) → {Boolean}

キーリピート状態か

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyName` | [String](String.md) | キー名称 |


##### Returns:

<dl>
	<dt> Type </dt>
	<dd>
		<span>Boolean</span>
	</dd>
</dl>

#### (static) isTriggered (keyName) → {Boolean}

押された直後か

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `keyName` | [String](String.md) | キー名称 |


##### Returns:

<dl>
	<dt> Type </dt>
	<dd>
		<span>Boolean</span>
	</dd>
</dl>

#### (static) update ()

アップデート


 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
