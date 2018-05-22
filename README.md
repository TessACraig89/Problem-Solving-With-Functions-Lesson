# Problem Solving with Functions

<hr>
Title: Morning Lab<br>
Creator: Alex White<br>
Topics: Problem solving with functions<br>
<hr>

## Morning Lab - Problem solving

### printGreeting

Write a function called `printGreeting` with a parameter `name` that returns a greeting with the argument **interpolated** into the greeting.

```javascript
console.log(printGreeting("Slimer"));
```
> => Hello there, Slimer!

My Solution:

```javascript
const printGreeting = (name) => {
   console.log('Welcome ' + name);
}

printGreeting('jennifer');
``` 
<br>
<hr>

### reverseWordOrder

Write a function `reverseWordOrder` that accepts a single argument, a string. The function should return a string with the order of the words reversed. Don't worry about punctuation.

```javascript
console.log(reverseWordOrder("Ishmael me Call"));
```

> => "Call me Ishmael"


```
console.log(reverseWordOrder("I use Lâncome on my comb"));
```

> => "comb my on Lâncome use I"

My Solution:

```javascript
const reverseWordOrder = (str) => {
    // Step 1. Use the split() method to return a new array
    var splitString = str.split(" "); 
    // Step 2. Use the reverse() method to reverse the new created array
    var reverseArray = splitString.reverse();
    //Step 4. Return the reversed string
    return reverseArray;
 };

reverseWordOrder("hello there bill");
``` 
<br>
<hr>

### calculate

Write a function called `calculate`.

This function should take three arguments, two numbers and a string.

Name the parameters `num1`, `num2`, and `operation`.

If the function receives the string "add" for the operation parameter, it will return the sum of num1 and num2.

If the function receives the string "sub" for the operation parameter, it will return num1 minus num2.

Do the same thing for multiplication "mult", division "div", and exponent "exp" (where num2 is the exponent of num1).

```javascript
console.log(calculate(4, 3, "sub"));

=> 1
```

```javascript
console.log(calculate(4, 3, "exp"));

=> 64
```

<br>
<hr>

### pandigital numbers

A number of length n is _1-to-n pandigital_ if it makes use of all the digits 1 to n exactly once.

- The number `15234` is _1-to-n pandigital_.

- The number `333` is **not** _1-to-n pandigital_.

- The number `0` is **not** _1-to-n pandigital_.

- The number `987654321` is _1-to-n pandigital_.


Write a function that checks if a number is _1-to-n pandigital_.
