# $defer
Prioritizes sending the response. This is for codes that may take longer than 3 seconds to run, because Discord returns a error if the bot doesn't respond to a interaction (e.g slash commands) within the first 3 seconds.
> This should only be used for slash commands/interactions.

## Usage
```
$defer[ephemeral (yes/no) (optional)]
```

### Breakdown
`ephemeral` - Whether the response will be ephemeral or not. 'yes' means the response will be ephemeral, 'no' means it won't. Optional.
