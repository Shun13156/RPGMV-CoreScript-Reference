# Class: Item

## namespace [RPG](RPG.md)

アイテムの情報を記述したJSONデータ。ファイル data/Items.json に記述されている。

 [$dataItems](global.md#dataitems-arrayrpgitem) に配列として格納されている。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `itypeId` | [Number](Number.md) | [アイテムタイプ]のID (下表を参照) |
| `price` | [Number](Number.md) | [価格] |
| `consumable` | Boolean | [消耗]するか |

##### itypeId

| ID | [アイテムタイプ] |
| --- | --- |
| 1 | 通常アイテム |
| 2 | 大事なもの |
| 3 | 隠しアイテムA |
| 4 | 隠しアイテムB |


### Extends

* [RPG.UsableItem](RPG.UsableItem.md)

 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
