/*
Title: Functions
Description: Questions about functions in JS
*/

Function in JS are first class citizens and you should know them well (assigned to a variable, passed as an argument, returned from another, etc.).

**Output of this:**

```javascript
console.log(square(5));
/* ... */
function square(n) { return n * n; }
```

**Output of this:**

```javascript
console.log(square(5));

var square = function(n) {
  return n * n;
}
```

**Why do you do this?**

```javascript
var simpleLibrary = function() {
   var simpleLibrary = {
        a,
        b,
        add: function(a, b) {
            return a + b;
        },
        subtract: function(a, b) {
            return a - b;   
        }
   }
  return simpleLibrary;
}();
```

If more than one parameter has the same name in a function definition, the last occurrence “shadows” the preceding occurrences. [Ref](https://eslint.org/docs/rules/no-dupe-args)

## Function references

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions
