# Array Reduce Function
## Introduction
The array.reduce method takes an array of items and returns a single item, based on the logic contained in the provided function. The reduce method operates similar to an accumulating for loop, by cycling through each item, applying an operation on them, and keeping track of an accumulator throughout the process.
<br>
MDN documentation: [Array.Reduce MDN docs](developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)
<hr />

## Example

```javascript
//Collapse an array of object product and count values into a single object
var array = [{ product: "pickles", count: 9 }, 
            { product: "onions", count: 12 }, 
            { product: "olives", count: 4 }];
		
function reduceArray (a) {
    return a.reduce((acc, curr) => {
            acc[curr.product] = curr.count;
            return acc;
        }, {});
}
console.log(reduceArray(array));
```
## Result:

[Result]: ./Screenshot.png "Code Result"

