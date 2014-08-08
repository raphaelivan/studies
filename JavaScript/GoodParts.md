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


### Expressions
The simplest expressions are literal value: string, number, a variable, true, false, null, undefined, NaN, Infinity, an invocation expresion preceded by new,an expression wrapped in parentheses, an expression preceded by prefix or infix operator;

##### The operator precedence list:
  *Refinement and invocation* `.` `[]` `()`

  *Unary operators* `delete` `new` `typeof` `+` `-` `!`

  *Multiplication, division, remaider* `*` `/` `%`

  *Adition/cacatenation, substration* `+` `-`

  *Inequality* `>=` `<=` `><`

  *Equality* `===` `==` `!==` `!=`

  *Logical and* `&&`

  *Logical or* `||`

  *Ternary* `?:`

* [Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

## Objects
  The simples types of JavaScript are numbers, strings, booleans, null and undefined. All other values are objects.
  Numbers, strings and booleans are object-like in that the have methods, but they are immutable.

  Object in JavaScript are  class-free.

### Object Literals
  Object literals provide a very convenient notation for creating new object values.

  An object literal is a pair of culy braces.

```js
  var empty_object = {};

  var raphael = {
    name: 'Raphael Ivan',
    age: 24
  }
```
### Retrieval
Values can be retrivied from an object by wrapping a string expression in a [] sufix. If the string expression is a string literal and if it is a legal JavaScript name and not a reserved word, then the . notation can be used instead.

```js
  raphael.name;
  raphael['age'];
  raphael.nickname; //undefined
```

### Reference
  Objects are passed arround by references. They are **never** copied.
```js
  var a, b, c = {}; //refer to the same empty object;
```

### Prototype
 Every object is linked to a prototype object from which it can inherit properties. All literal object are linked to Object.prototype that comes standard with JavaScript.

 When you make a new object,  you can select the object that should be its prototype.

 > The prototype link has no effect on updating. It is used only in retrieval.

### Delete
The delete operator can be used to remove a property from an object.
```js
  delete App.init;
```
Removing a property from an object may allow a property from prototype linkage to shine through

* [Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)


References:
* [JavaScript The Good Parts Book](http://shop.oreilly.com/product/9780596517748.do)