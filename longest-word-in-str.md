###4.Find the Longest Word in a String

Return the length of the longest word in the provided sentence.

Your response should be a number.

Remember to use Read-Search-Ask if you get stuck. Write your own code.

*New Working Version*


```javaScript
function findLongestWord(str) {
return str.split(" ").reduce((prev, curr) => (prev.length > curr.length) ? prev : curr).length;

}

findLongestWord("The quick brown fox jumped over the lazy dog");
```

I accidentally saved my new version without first copying the original :(
