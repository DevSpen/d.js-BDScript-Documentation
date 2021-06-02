# $data
Pulls data from given assigned values from a function.
> Example of $data: `$cooldown[30s;Please wait $data[time] until using that command again!]`.

## Usage
```
$data[property;(optional) hideError (yes/no)]
```

### Breakdown
`property` - The name of the property that holds the data.

`hideError` - Whether to suppress the error if data does not exist or not. 'yes' means the errors are suppressed, 'no' means they are not. 'no' is default, optional.
