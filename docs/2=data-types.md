# data types

- primitives
  - primary
    - number
    - string
    - boolean
  - special
    - undefined
    - null
    - symbol
- composite
  - arrays
  - objects

## number

- can be negative or positive, integer or decimal
- can be expressed in octal, hexadecimal or binary (prefixing)
- calculation outside js range will give plus minus infinity
- invalid operation to number (ie divide by string) will give "NaN"
  - nothing is equal to NaN, not even itself
  - use js built-in function `isNaN()` to check

```js
let number = 1;
let oct = 0o77; // 63
let hx = 0x0011; // 17
let bin = 0b1100; //12
```

## string

- sequence of chars within quotes
  - single quotes (use back-slash to escape inline quotes)
  - double quotes
  - back ticks (new to ES2015)
    - mutiline strings, perserve linebreaks

```js
let str = "there is nothing I can't do";
let joined = "wait, " + "what?";
let multiline = "new\nline";
let mulitine2 = `new
line`;
```

## boolean

- has the value true or false (literal)
- truthy or falsy (false, 0, "", null, undefined, NaN)

## null and undefined

- a variable that is declared but unassighed - undefined
- once declared, a variable cannot be un-declared
- undefined is a lack of value
- we can set variable to null anytime
- null is a value of nothing

## symbol

- has no constructor function, can't use "new" keyword
- need to use a global function, that is capitalized

```js
let mySymbol = Symbol();
let mySymbol = Symbol("desc for debug purposes");
```

- purpose - use as keys in an object
- symbols are always unique
- we can add new key to object with a symbol, and know it won't overwrite existing keys

```js
let sym1 = Symbol("x");
let sym2 = Symbol("x");
console.log(sym1 === sym2); // false
```

## array

- indexes based on numbers

```js
let array = [5, "something", true];
let array2 = new Array(); // rarely used
array[0]; // 5
```

## objects

- containers for key-value pairs of data
- indexes based on words

```js
let obj = {
  num: 5,
  str: "whoo",
};
obj.num; // 5 - dot notation
obj["str"]; // whoo - bracket notation
```
