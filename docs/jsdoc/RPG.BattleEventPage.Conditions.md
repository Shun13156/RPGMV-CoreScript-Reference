# Class: Conditions

## Namespace: [RPG](RPG.md).[BattleEventPage](RPG.BattleEventPage.md)

敵グループの [EVページ] の [条件] を構成するJSONデータ。

[RPG. BattleEventPage](RPG.BattleEventPage.md) の conditions プロパティに含まれる。

類似のクラスに [RPG.EventPage.Conditions](RPG.EventPage.Conditions.md)、[RPG.CommonEvent](RPG.CommonEvent.md) がある。 

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `turnEnding` | Boolean | [ターン終了] を使うか |
| `turnValid` | Boolean | [ターン] を使うか |
| `turnA` | [Number](Number.md) | [ターン] + の前の数値 |
| `turnB` | [Number](Number.md) | [ターン] + の後の数値  |
| `enemyValid` | Boolean | [敵キャラHP] を使うか |
| `enemyIndex` | [Number](Number.md) | [敵キャラHP] の敵キャラ番号 |
| `enemyHp` | [Number](Number.md) | [敵キャラHP] \(%) |
| `actorValid` | Boolean | [アクターHP] を使うか |
| `actorId` | [Number](Number.md) | [アクターHP] のアクターID |
| `actorHp` | [Number](Number.md) | [アクターHP] \(%) |
| `switchValid` | Boolean | [スイッチ] を使うか |
| `switchId` | [Number](Number.md) | [スイッチ] のID |

 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
