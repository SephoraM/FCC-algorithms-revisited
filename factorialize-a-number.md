### 2.Factorialize a Number



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
    return Array.from(new Array(num),(val,index)=>index+1).reduce((prev, curr) => prev * curr);
  }
```  
