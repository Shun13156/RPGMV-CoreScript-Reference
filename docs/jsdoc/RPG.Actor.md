# Class: Actor

## Namespace: [RPG](RPG.md)

 アクターを記述したファイル( data/Actors.json )のJSONデータ。

 大域変数 [$dataActors](global.md#dataactors-arrayrpgactor) に配列として格納されている。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `id` | [Number](Number.md) | ID |
| `name` | [String](String.md) | [名前] |
| `nickname` | [String](String.md) | [二つ名] |
| `classId` | [Number](Number.md) | [クラス]ID |
| `initialLevel` | [Number](Number.md) | [初期レベル] |
| `maxLevel` | [Number](Number.md) | [最大レベル] |
| `characterName` | [String](String.md) | [歩行キャラ]画像ファイル名 |
| `characterIndex` | [Number](Number.md) | 8分割された[歩行キャラ]画像のひとつを指定する番号(0 〜 7) |
| `faceName` | [String](String.md) | [顔]画像のファイル名 |
| `faceIndex` | [Number](Number.md) | 8分割された[顔]画像のひとつを指定する番号(0 〜 7) |
| `battlerName` | [String](String.md) | [[SV]戦闘キャラ]画像ファイル名 |
| `equips` | [Array](Array.md).<[Number](Number.md)> | [初期装備](装備品 ID の配列) |
| `profile` | [String](String.md) | [プロフィール]の文 |
| `traits` | [Array](Array.md).<[RPG.Trait](RPG.Trait.md)> | [特徴]の配列 |


### Extends

* [RPG.MetaData](RPG.MetaData.md)

 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
