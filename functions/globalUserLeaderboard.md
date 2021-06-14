# $globalUserLeaderboard
Makes a global user leaderboard.

## Usage
```
$globalUserLeaderboard[variableName;sortType (asc/desc);customText;(optional) separator;(optional) page;(optional) limit]
```

### Breakdown
`variableName` - The name of the variable to create the leaderboard for.

`sortType` - Whether to sort the leaderboard in ascending (`asc`) or descending (`desc`) order. 

![image](https://user-images.githubusercontent.com/69215413/121826883-0e273080-cc88-11eb-9b1f-abe8a27b2288.png)

`customText` - What to display for each new placement on the leaderboard. [(view all leaderboard properties)](https://djs-bdscript.gitbook.io/docs/properties/leaderboard-properties)

Example: `$data[position] | $data[tag] - $data[value]`

Output: `1 | User#0000 - 100`

`separator` - The separator between placements. Default is `\n` (new line). Optional.

`page` - Which page to display. Default is first page (`1`). Optional.

`limit` - How many placements to display on each `page`. Default is `10`. Optional.

## Example
```js
bot.command({
    type: "command",
    name: "leaderboard",
    code: `$description[$globalUserLeaderboard[Money;asc;$data[position] | $data[tag] - $data[value]]
]`
})
```

