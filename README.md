# What-I-Learned-In-Week-4

### Boolean
Boolean is a datatype that returns either of two values i.e. true or false. 
```
const isHungry = true;
const hasMoney = false;
const hasFridge = false;
console.log(isHungry || hasFridge && hasMoney);
```
* `&&` is a binary operator
* The computer will execute && first and then ||
* `===` (**strict** equality) will check if the both the ##type## and the ##value## are the same.
  * i.e. `5 === 5` *true*
* `==` (**loose** equality) also performs a **type coercion**. Type coercion means that two values are compared only after attempting to convert them into a common type.
  * i.e. `'5' == 5` *true*
* `!==` (**non-identity** operator) returns true if the operands **are not equal and/or not of the same type**.
* `>, < or <= >=` 
  * i.e. `console.log(3 <= 5)`