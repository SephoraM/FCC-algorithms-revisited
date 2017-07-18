### 1. Reverse a String



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
