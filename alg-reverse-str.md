### 1. Reverse a String

Reverse the provided string.

You may need to turn the string into an array before you can reverse it.

Your result must be a string.

*Original Working Version*

```JavaScript
function reverseString(str) {
  str = str.split(""); //turns into array
  str = str.reverse(); // reverses order of array
  str = str.join("");  // turns into string
  return str;
}

reverseString("hello");
```
*New Working Version*

```JavaScript
  function reverseString(str) {
    return str.split("").reverse().join("");
  }
```

*Or with arrow syntax*

```JavaScript
  let reverseString = (str) => str.split("").reverse().join("");
```  
