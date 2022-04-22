# Web-Skills-with-Shikmamaru(4)
![Shikamaru](https://github.com/whitebird1016/Web-Skills-with-Shikmamaru/blob/main/1_HTGSqvOc52yfMwyLhCMjVA.jpeg)
<h2>Array Skills</h2>
<h3>1: Clone array</h3>

```
const _arr = [0, 1, 2];
const arr = [..._arr];
// arr => [0, 1, 2]
```
<h3>2: Merge array</h3>

```
const arr1 = [0, 1, 2];
const arr2 = [3, 4, 5];
const arr = [...arr1, ...arr2];
// arr => [0, 1, 2, 3, 4, 5];
```
<h3>3:  Deduplicated array</h3>

```
const arr = [...new Set([0, 1, 1, null, null])];
// arr => [0, 1, null]
```
<h3>4: Obfuscated array</h3>

```
const arr = [0, 1, 2, 3, 4, 5].slice().sort(() => Math.random() - .5);
// arr => [3, 4, 0, 5, 1, 2]
```
<h3>5: Empty an array</h3>

```
const arr = [0, 1, 2];
arr.length = 0;
// arr => []
```
<h3>6: Truncate array</h3>

```
const arr = [0, 1, 2];
arr.length = 2;
// arr => [0, 1]
```
<h3>7: Exchange assignment</h3>

```
let a = 0;
let b = 1;
[a, b] = [b, a];
// a b => 1 0
```
<h3>8: Filter empty values</h3>

```
const arr = [undefined, null, "", 0, false, NaN, 1, 2].filter(Boolean);
// arr => [1, 2]
```
<h3>9: Insert member at the beginning of the array</h3>

```
let arr = [1, 2];
arr.unshift(0);
arr = [0].concat(arr);
arr = [0, ...arr];
// arr => [0, 1, 2]
```
<h3>10: Insert members at the end of the array</h3>

```
let arr = [0, 1]; 
arr.push(2);
arr.concat(2);
arr[arr.length] = 2;
arr = [...arr, 2];
// arr => [0, 1, 2]
```
<h3>11: Count number of array members</h3>

```
const arr = [0, 1, 1, 2, 2, 2];
const count = arr.reduce((t, v) => {
 t[v] = t[v] ? ++t[v] : 1;
 return t;
}, {});
// count => { 0: 1, 1: 2, 2: 3 }
```

<h3>12: Destructuring nested array members</h3>

```
const arr = [0, 1, [2, 3, [4, 5]]];
const [a, b, [c, d, [e, f]]] = arr;
// a b c d e f => 0 1 2 3 4 5

```

<h3>13: Destructuring array member aliases</h3>

```
const arr = [0, 1, 2];
const { 0: a, 1: b, 2: c } = arr;
// a b c => 0 1 2
```

<h3>14: Destructuring array member default value</h3>

```
const arr = [0, 1, 2];
const [a, b, c = 3, d = 4] = arr;
// a b c d => 0 1 2 4
```

<h3>15: Get random array member</h3>

```
const arr = [0, 1, 2, 3, 4, 5];
const randomItem = arr[Math.floor(Math.random() * arr.length)];
// randomItem => 1
```

<h3>16: Create an array of specified length</h3>

```
const arr = [...new Array(3).keys()];
// arr => [0, 1, 2]
```

<h3>17: Creates an array of the specified length and equal values</h3>

```
const arr = new Array(3).fill(0);
// arr => [0, 0, 0]
```
