# $formatDate
Converts milliseconds to a readable date/time.

## Usage
```
$formatDate[milliseconds;format]
```

### Breakdown
`milliseconds` - The milliseconds to convert.
`format` - The format of the date. 

## Example Formats
```js
MMMM Do YYYY, h:mm:ss a
// June 5th 2021, 11:35:22 am
```
```js
dddd
// Saturday
```
```js
MMM Do YY
// Jun 5th 21
```
```js
empty
// 2021-06-05T11:37:54-04:00
```
[See more.](https://momentjs.com/)

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Creation Date: $formatDate[$creationDate[$mentioned[1;yes]];MMMM Do YYYY, h:mm:ss a]`
})
```
