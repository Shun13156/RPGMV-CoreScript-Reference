# Class: Skill

## namespace [RPG](RPG.md)

スキルの情報を記述したJSONデータ。

ファイル data/Skills.json に記述されている。

[$dataSkills](global.md#dataskills-arrayrpgskill) に配列として格納されている。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `stypeId` | [Number](Number.md) | [スキルタイプ]のID (下表を参照) |
| `mpCost` | [Number](Number.md) | [消費MP] |
| `tpCost` | [Number](Number.md) | [消費TP] |
| `message1` | [String](String.md) | 上段[メッセージ] |
| `message2` | [String](String.md) | 下段[メッセージ] |
| `requiredWtypeId1` | [Number](Number.md) | [必要武器]の[武器タイプ1] |
| `requiredWtypeId2` | [Number](Number.md) | [必要武器]の[武器タイプ2] |


##### stypeId

[データベース]-[タイプ]-[スキルタイプ] で設定されたID。

 [System](RPG.System.md) の skillTypes プロパティに登録されている。
 
 下表はデフォルトの値。

| ID | [スキルタイプ] |
| --- | --- |
| 0 | なし |
| 1 | 魔法 |
| 2 | 必殺技 |

### Extends

* [RPG.UsableItem](RPG.UsableItem.md)

 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
