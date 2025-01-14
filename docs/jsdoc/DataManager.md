# Class: DataManager

 データベースの管理を行う静的クラス。 セーブデータの管理など行う。だいたい、$XXXで大域変数に設定されているものの管理。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `_globalId` | [String](String.md) | [static]システムID 'RPGMV' |
| `_lastAccessedId` | [Number](Number.md) | [static]最後にセーブ・ロードを行ったファイルのID |
| `_errorUrl` | * | [static] |
| `_databaseFiles` | [Array](Array.md).\<Object> | [static]読み込むデータファイル情報(Object例:{ name: '$dataXxx', src: 'Xxx.json'}) |


### Methods

#### (static) checkError ()
 エラーが記録されていれば、エラーを表示。


#### (static) createGameObjects ()
$game から始まる大域変数に、対応したオブジェクトを生成し代入。


#### (static) extractMetadata (data)
data.noteに書いてあるデータを分解しdata.metaに設定。<br />
渡したdata自体が書き換えられるので、返り値はない。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `data` | Object | [RPG.MetaData](RPG.MetaData.md) |


#### (static) extractSaveContents (contents)
 渡したオブジェクトから$gameで始まる大域変数に値を返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `contents` | Object |  |


#### (static) isAnySavefileExists () → {Boolean}
 セーブファイルが(ひとつでも)存在するか。


#### (static) isArmor (item) → {Boolean}
 指定した項目が[防具]に含まれるか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `item` | object |  |


#### (static) isBattleTest () → {Boolean}
[戦闘テスト]モードか。


#### (static) isDatabaseLoaded () → {Boolean}
 データベースの読み込みが完了しているか。


#### (static) isEventTest () → {Boolean}
[イベントテスト]モードか。


#### (static) isItem (item) → {Boolean}
 指定した項目が[アイテム]に含まれるか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `item` | Object |  |


#### (static) isMapLoaded () → {Boolean}
 マップの読み込みが完了しているか。


#### (static) isSkill (item) → {Boolean}
 指定した項目が[スキル]に含まれるか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `item` | Object |  |


#### (static) isThisGameFile (savefileId) → {Boolean}
 指定した ID のセーブファイルが存在するか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) isWeapon (item) → {Boolean}
 指定した項目が[武器]に含まれるか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `item` | object |  |


#### (static) lastAccessedSavefileId () → {[Number](Number.md)}
 最後にセーブ・ロードを行ったファイルのIDを返す。


#### (static) latestSavefileId () → {[Number](Number.md)}
 最新のセーブファイルID を返す。


#### (static) loadAllSavefileImages ()
 全てのセーブファイルの画像を読み込む。


#### (static) loadDatabase ()
 データベースファイル( $data から始まる大域変数に代入される JSON)を読み込む。 ただし $dataMap は別扱い。


#### (static) loadDataFile (name, src)
 指定したデータを読み込む。読み込みが完了したら onLoad が呼ばれる。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `name` | [String](String.md) |  データ代入先の大域変数名 $dataXXX |
| `src` | [String](String.md) | data/以下のファイル名 |


#### (static) loadGame (savefileId)
 指定したセーブファイルID からデータを読み込む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) loadGameWithoutRescue (savefileId) → {Boolean}
 指定したセーブファイルID からリソース抜きの情報を読み込み、 読み込みに成功したか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) loadGlobalInfo () → {[Array](Array.md).<[MV.SaveFileInfo](MV.SaveFileInfo.md)>}
GlobalInfo を読み込んで返す。


#### (static) loadMapData (mapId)
 マップデータを読み込む。完了時は onLoad が呼ばれる。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `mapId` | [Number](Number.md) | 1: 空のマップを作る |


#### (static) loadSavefileImages (info)
 セーブファイルに必要な画像を読み込む。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `info` | Object |  |


#### (static) loadSavefileInfo (savefileId) → {Object}
 指定したセーブファイルID の情報を読み込んで返す。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) makeEmptyMap ()
 空のマップを作成。


#### (static) makeSaveContents () → {Object}
 セーブ用のデータ作成。$gameで始まる大域変数をまとめたオブジェクトを返す。 ただし$gameTemp, $gameMessage, $gameTroop を含まない。


#### (static) makeSavefileInfo () → {[MV.SaveFileInfo](MV.SaveFileInfo.md)}
 新規のセーブファイル情報を作って返す。


#### (static) maxSavefiles () → {[Number](Number.md)}
 セーブ可能なファイルの最大数を返す。


#### (static) onLoad (object)
 データ読み込み完了時に呼ばれるハンドラ。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `object` | * |  データを格納したオブジェクト |


#### (static) saveGame (savefileId) → {Boolean}
 ゲームデータをセーブファイルに保存し、 保存に成功したか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) saveGameWithoutRescue (savefileId) → {Boolean}
 指定したセーブファイルID にリソース抜きの情報を保存し、 保存に成功したか。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `savefileId` | [Number](Number.md) |  |


#### (static) saveGlobalInfo (info)
GlobalInfo を保存。

##### Parameters:

| Name | Type | Description |
| --- | --- | --- |
| `info` | [MV.SaveFileInfo](MV.SaveFileInfo.md) |  |


#### (static) selectSavefileForNewGame ()
[ニューゲーム]用のセーブファイルを選択。


#### (static) setupBattleTest ()
[戦闘テスト] の準備。


#### (static) setupEventTest ()
[イベントテスト]の準備。


#### (static) setupNewGame ()
 新規ゲームの準備。


 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
