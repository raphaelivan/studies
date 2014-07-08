JavaScript The Good Parts
==============================
## Grammar

### Whitespace
Whitespace is usually insignificant, butit is occassionally necessary to use whitespace to separate sequence of characters.

```js
  var that = this;
```
### Names
A name is a letter optionally followed by one or more letters, digits, or underbars. A name cannot be one reserved word.
* [Reserved Words](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords)

### Numbers
JavaScript represent numbers, internally, as 64-bit floating point. Unlike most other programming languages, there is no separete integer types, so 1 and 1.0 are the same value.

### Strings
String are immutable. Once it is made, a string can never be changed.

### Statements
A compilation unit contains a set of executable statements. In web browsers, each script tag delivery a compilation unit that is compiled and immediatly executed. JavaScript throws them all together in a common global namespace.

Blocks in JavaScript do not create scope.

Falsy values: false, null, 0, '', NaN, undefined; All other values are truthy

References:
* [JavaScript The Good Parts Book](http://shop.oreilly.com/product/9780596517748.do)