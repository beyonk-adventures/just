## just-clone

Part of a [library](../../../../) of zero-dependency npm modules that do just do one thing.  
Guilt-free utilities for every occasion.

[Try it now](http://anguscroll.com/just/just-extend)

```js
// Identical to `just-extend(true, {}, obj1)`

import clone from 'just-clone';

var arr = [1, 2, 3];
var subObj = {aa: 1};
var obj = {a: 3, b: 5, c: arr, d: subObj};
var objClone = clone(obj);
arr.push(4);
subObj.bb = 2;
obj; // {a: 3, b: 5, c: [1, 2, 3, 4], d: {aa: 1}}  
objClone; // {a: 3, b: 5, c: [1, 2, 3], d: {aa: 1, bb: 2}}
```