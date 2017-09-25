# random-js-snippets
cool es6/es7 syntax

# using the rest operator to destructure objects
I found the es7 rest feature to be pretty cool.

```javascript
const obj = {
  apples: 1,
  oranges: 23,
  lemons: 31,
  tomatoes: 12
}
const {apples, tomatoes, ...restOfThem} = obj; // wow es7!
console.log(restOfThem);
```
The output for the above code will be

```
{ oranges: 23, lemons: 31 }
```
The order of the variables for the input doesn't matter as well, i.e, `const {tomatoes, apples, ...restOfThem} = obj` produces the same output. The only caveat is that the rest element has to be the last element when destructuring.
  
