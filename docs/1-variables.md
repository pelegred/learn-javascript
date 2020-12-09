# variables

```js
var foo; // undefined
```

# variable names

- can use any letter, number, or underscore (rarely $)
- can't start with numbers
- case sensitive
- can't be one of javascript's reserved keywords

```js
var foo, bar, baz;
var foo = 42;
```

- you can intialize variable (assign a value) with = sign
- can declare many using comma
- js is weakly / dynamicaly type language

## var, let, const

- var keyword - can create variable in the global scope
- let keyword - only visible inside a "block", is block-scoped
- const keyword - cannot changed through reassignment

## a little about scope

- scopes - global, function, block
- global - can be accessed fro anywhere (useful for libraries, but can break your app)
- function - only visible to function declared it
- block - enclosed with curly braces `{}`
