# Switch  
  
# Rewrite the "switch" into an "if"  
```
switch (browser) {
  case 'Edge':
    alert( "You've got the Edge!" );
    break;

  case 'Chrome':
  case 'Firefox':
  case 'Safari':
  case 'Opera':
    alert( 'Okay we support these browsers too' );
    break;

  default:
    alert( 'We hope that this page looks ok!' );
}
```
  
```
if (case === 'Edge') {
    alert( "You've got the Edge!" );
} else if (case === '' || case === 'Firefox' || case === 'Safari' || case === 'Opera') {
    alert( 'Okay we support these browsers too' );
} else {
   alert( 'We hope that this page looks ok!' );
}
```
  

# Rewrite "if" into "switch"  
```
let a = +prompt('a?', '');

if (a == 0) {
  alert( 0 );
}
if (a == 1) {
  alert( 1 );
}

if (a == 2 || a == 3) {
  alert( '2,3' );
}
```
  
```
let a = +prompt('a?', '');

switch(a) {
    case 0:
        alert( 0 );
        break;
    case 1:
        alert( 1 );
        break;
    case 2:
    case 3:
        alert( '2,3' );
        break;
}
```
  