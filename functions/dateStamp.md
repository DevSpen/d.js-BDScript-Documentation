# $dateStamp
Returns current date since 1970 in ms.


## Usage
`$dateStamp`


## Example
```bot.command({
 type: "command",
 name: "date",
 code: `$description[Check the date below!]
$dateStamp`
 })````
