### 3.Check For Palindromes



*Original Working Version*

```JavaScript
  function palindrome(str) {
    // Good luck!
    str = str.replace(/[\W_]+/g, ""); // using regular expressions and replace
    str = str.toLowerCase();
    var newStr = [];
    newStr = str.split("").reverse().join(""); //split into an array, reverse elements, join into string
    if (newStr === str) { // check if reversed matches original
      return true;
    }

    return false;
  }

palindrome("eye");
```

*New Working Version*

Barely changed this. Just tidied it up a little.

```JavaScript
  function palindrome(str) {
    let newStr = str.replace(/[\W_]+/g, "").toLowerCase();
    let reversedString = newStr.split("").reverse().join("");
    if (newStr === str) { // check if reversed matches original
      return true;
    }

    return false;
  }
```  
