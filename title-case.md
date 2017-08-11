###5.Title Case a Sentence

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".

*Original Working Version*

```JavaScript

function titleCase(str) {
  str = str.toLowerCase(); // make lower case
  str = str.split(" "); //split into array

  for (var i = 0; i < str.length; i++) { //iterate through array
    str[i] = str[i].charAt(0).toUpperCase() + str[i].slice(1); // each element, first char to upper case
                                                               // concat the rest of word, move to next elem
  }
 return str.join(" ");// return as string
}

titleCase("I'm a little tea pot");
```

*New Working Version*

```JavaScript
function titleCase(str) {
  let arr = str.toLowerCase().split(" "); //split into array

  return arr.map(elem => elem.charAt(0).toUpperCase() + elem.slice(1)).join(" ");
     // each element, first char to upper case


}

titleCase("I'm a little tea pot");
```
