# Logical operator  
  
### What's the result of OR?  
    alert( null || 2 || undefined );            // 2 (first true statement)

### What's the result of OR'ed alerts?  
    alert( alert(1) || 2 || alert(3) );         // 2: alert(1) return `undefined`

### What is the result of AND?  
    alert( 1 && null && 2 );                    // null (first false statement)

### What is the result of AND'ed alerts?  
    alert( alert(1) && alert(2) );              // undefined

### The result of OR AND OR  
    alert( null || 2 && 3 || 4 );               // 3: evalueted `2 && 3 → 3` and then `null || 3 || 4`

### Check the range between  
Write an if condition to check that age is between 14 and 90 inclusively.  
“Inclusively” means that age can reach the edges 14 or 90.
    if (age>=14 && age<=90) { ... }

### Check the range outside  
Write an if condition to check that age is NOT between 14 and 90 inclusively.  
Create two variants: the first one using NOT !, the second one – without it.
1. if (!(age>=14 && age<=90)) { ... }
2. if (age<14 || age>90) { ... }

### A question about "if"  
    if (-1 || 0) alert( 'first' );              // `first`          condition: -1, true
    if (-1 && 0) alert( 'second' );             // don't evalueted  condition: 0, false
    if (null || -1 && 1) alert( 'third' );      // `third`          condition: `-1 && 1 = 1` then `null || 1 = 1`, true

