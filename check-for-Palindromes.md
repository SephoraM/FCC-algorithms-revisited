### 3.Check For Palindromes

Return true if the given string is a palindrome. Otherwise, return false.

A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.

Note
You'll need to remove all non-alphanumeric characters (punctuation, spaces and symbols) and turn everything lower case in order to check for palindromes.

We'll pass strings with varying formats, such as "racecar", "RaceCar", and "race CAR" among others.

We'll also pass strings with special symbols, such as "2A3*3a2", "2A3 3a2", and "2_A3*3#A2".

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
