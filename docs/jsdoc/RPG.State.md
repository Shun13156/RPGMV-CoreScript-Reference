# Class: State

## namespace [RPG](RPG.md)

ステートを記録したJSONデータで、ファイル data/States.json に記録されている。

読み込まれたデータは、[$dataStates](global.md#datastates-arrayrpgstate) に配列として格納されている。

##### Properties:

| Name | Type | Description |
| --- | --- | --- |
| `id` | [Number](Number.md) | ID |
| `name` | [String](String.md) | 名前 |
| `restriction` | [Number](Number.md) | Action restrictions. 0: None 1: Attack enemy 2: Attack enemy or ally 3: Attack ally 4: Cannot act |
| `priority` | [Number](Number.md) | The state priority (0..100). |
| `removeAtBattleEnd` | Boolean | Removes state at end of battle (true/false). |
| `removeByRestriction` | Boolean | Removes state by action restriction (true/false). |
| `autoRemovalTiming` | [Number](Number.md) | The timing of automatic state removal. 0: None 1: At end of action 2: At end of turn |
| `minTurns` | [Number](Number.md) | The minimum turns of the duration. |
| `maxTurns` | [Number](Number.md) | The maximum turns of the duration. |
| `removeByDamage` | Boolean | Removes state by damage (true/false). |
| `chanceByDamage` | [Number](Number.md) | Chance of state being removed by damage (%). |
| `removeByWalking` | Boolean | Removes state by walking (true/false). |
| `stepToRemove` | [Number](Number.md) | Number of steps until state is removed. |
| `iconIndex` | [Number](Number.md) | The icon number. |
| `message1` | [String](String.md) | The message when an actor fell in the state. |
| `message2` | [String](String.md) | The message when an enemy fell in the state. |
| `message3` | [String](String.md) | The message when the state remains. |
| `message4` | [String](String.md) | The message when the state is removed. |
| `motion` | [Number](Number.md) | The side-view motion. |
| `overlay` | [Number](Number.md) | The side-view overlay. |
| `traits` | [Array](Array.md).<[RPG.Trait](RPG.Trait.md)> | The array of Trait data. |

<dl>
</dl>

### Extends

* [RPG.MetaData](RPG.MetaData.md)

 <br>

  Documentation generated by [JSDoc 3.5.5](https://github.com/jsdoc3/jsdoc)
