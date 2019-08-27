# String repeat [link](https://www.codewars.com/kata/57a0e5c372292dd76d000d7e)
Write a function called repeatString which repeats the given String src exactly count times.
```js
repeatStr(6, "I") // "IIIIII"
repeatStr(5, "Hello") // "HelloHelloHelloHelloHello"
```
## learn repeat [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat)
<details><summary>Sopiler Alert</summary>
<code><pre>
function repeatStr (n, s) {
  return s.repeat(n);
}
// another
function repeatStr (n, s) {
  String.prototype.repeat = function(n) {
     return (new Array(n + 1)).join(this);
  };
  return s.repeat(n);
}
</pre></code></details>

## for / while loop
<details><summary>Sopiler Alert</summary><code><pre>
function repeatStr (n, s) {
var str="";
for(var i=0; i < n; i++)
  str+=s;
  return str;
}
// while loop
function repeatStr (n, s) {
  var myString = '';
  while(n > 0) {
    myString += s;
    n--;
  }
  return myString;
}
</pre></code></details>

[Go Back](../../index.md)
