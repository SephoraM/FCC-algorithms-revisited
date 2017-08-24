### 2.Factorialize a Number

Return the factorial of the provided integer.

If the integer is represented with the letter n, a factorial is the product of all positive integers less than or equal to n.

Factorials are often represented with the shorthand notation n!

For example: 5! = 1 * 2 * 3 * 4 * 5 = 120



*Original Working Version*

```JavaScript
function factorialize(num) {
var result = 1;    // starting with 1 because of the multiplication
for (var i = 1; i <= num; i++) {
  result *= i;

}
return result;
}

factorialize(5);
```

*New Working Version*


```JavaScript
  function factorialize(num) {
    return Array.from(new Array(num),(val,index) => index + 1).reduce((prev, curr) => prev * curr);
  }
```

 *Or using recursion*

 ```JavaScript
   function factorialize(num) {
     if(num === 1) {
       return num;
     } else {
       return num *= factorialize(num -1);
     }
   }
 ```
