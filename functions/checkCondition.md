# $checkCondition
Simply put, $checkCondition serves as a way to make a true or false statement. For example:

Example: `$checkCondition[$username==Spen]`
The bot would return "true" if someone named Spen used the command, otherwise it would return "false".

However, if I made $checkCondition say this: $checkCondition[$username!=Spen] 
Then it would return "false" if someone named Spen used the command, otherwise it would return "true".

## Usage
```$checkCondition[value(sign)value] ```

### Whats Sign?
• Replace (sign) with one of these 
== - Must be equal 
!= - Must be not equal 
< Must be less than (only numbers) 
> - Must be greater than (only numbers) 
=> - Must be greater than or equal to (only numbers) 
<= - Must be less than or equal to (only numbers) 
