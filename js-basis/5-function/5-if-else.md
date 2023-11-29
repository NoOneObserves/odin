# Is "else" required?
The following function returns true if the parameter age is greater than 18.

Otherwise it asks for a confirmation and returns its result:
```
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm('Did parents allow you?');
  }
}
```

1. Will the function work differently if `else`` is removed?
```
function checkAge(age) {
  if (age > 18) {
    return true;
  }
  // ...
  return confirm('Did parents allow you?');
}
```

2. Is there any difference in the behavior of these two variants?


## Solution
1. The function would work similiarly but it would return `undefined` instead of 'Did parents allow you?'.
2. These two function have the same behavior but they difference in how the code is structured. In the function without the else statement, the subsequent code `return confirm(...)`` will be executed whether the condition is true or false. In the other one, the else block will only be executed if the condition is false.