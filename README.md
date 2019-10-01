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
* **The computer will execute && first and then ||.**
* `===` (**strict** equality) will check if the both the ##type## and the ##value## are the same.
  * i.e. `5 === 5` *true*
* `==` (**loose** equality) also performs a **type coercion**. Type coercion means that two values are compared only after attempting to convert them into a common type.
  * i.e. `'5' == 5` *true*
* `!==` (**non-identity** operator) returns true if the operands **are not equal and/or not of the same type**.
* `>, < or <= >=` 
  * i.e. `console.log(3 <= 5)`

### If/Else Statement
Conditional statements are used to perform different actions based on different conditions. In JavaScript we have the following conditional statements:
* Use `if` to specify a block of code to be executed, if a specified condition is true
* Use `else` to specify a block of code to be executed, if the same condition is false
* Use `else if` to specify a new condition to test, if the first condition is false
```
function grader(score) {
    let response = '';

    if (score > 77) {
        response = response + 'Good job! ';
    } else {
        response = response + 'Keep on trying! ';
    }
    if (score >= 90) {
        response = response + 'You got an A';
    } else if(score >=80) {
        response = response + 'You got a B';
    } else {
        response = response + 'You failed.';
    }

    return response;
}

console.log(grader(59));
```

### FizzBuzz
I enjoyed working in a group to come up with the solution to this exercise. We we're able to discuss the different possibilities by moving around the lines of code and using other test cases.
```
function fizzy(num) {
  if(num % 3 === 0 && num % 5 === 0) {
    return 'FizzBuzz';
  } else if(num % 3 === 0) {
    return 'Fizz';
  } else if(num % 5 === 0) {
    return 'Buzz';
  } else {
    return num;
  }
}
```


