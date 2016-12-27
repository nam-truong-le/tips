# JavaScript Best Practices

## Avoid global variables

## Avoid `==`, use `===`

## Avoid `eval()`

## Don't use `new Object()`

* Use `{}` instead of `new Object()`
* Use `""` instead of `new String()`
* Use `0` instead of `new Number()`
* Use `false` instead of `new Boolean()`
* Use `[]` instead of `new Array()`
* Use `/()/` instead of `new RegExp()`
* Use `function() {}` or `() => {}` instead of `new Function()`

```JavaScript
let x = "John";
let y = new String("John");
(x === y) // is false
```

## Use `"use strict"`

## Development code is not live code

## Anonymously scope JavaScript if you're never going to call it elsewhere

# Performance

## Excessive DOM changes

## Events that get fired all the time: resizing, scrolling,...

* `unbind()` all event handlers before binding.

## Lots of HTTP requests
