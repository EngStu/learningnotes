# Return Negative [link](https://www.codewars.com/kata/55685cd7ad70877c23000102)
In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

Example:
```js
makeNegative(1); // return -1
makeNegative(-5); // return -5
```
learn Math.abs() [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/abs)
<details><summary>Sopiler Alert</summary>
<code><pre>
function makeNegative(num) {
  return -Math.abs(num);
}
function makeNegative(num) {
  return Math.abs(num) * -1;
}
</pre></code>
</details>

conditional solution
<details><summary>Sopiler Alert</summary>
<code><pre>
function makeNegative(num) {
  if ( num > 0 ) {
        return -num;
    }
    else {
        return num;
    }
}
function makeNegative(num) {
  return num <= 0 ? num : num*-1;
}
</pre></code>
</details>

<details><summary>Sopiler Alert</summary>
<code><pre>
const makeNegative = (num) => num < 0 ? num : num > 0 ? -Math.abs(num): 0;
</pre></code>
</details>

[Go Back](../../index.md)
