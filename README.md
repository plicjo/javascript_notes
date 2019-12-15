
# Javascript Notes

## Undefined vs null

`undefined` means that a variable was explicitly NOT SET to anything. Aka nothing.
`null` means that a variable was explicity SET to NOTHING

## Access default params deep into a function
Say you have a function where you have 2 default arguments. You want to use the first one as default, but set the second value.

```javascript
function myName(first = 'Joshua', last = 'Plicque') {
  return `${first} ${last}`
}
```

By passing in `undefined` to the first value, you tell the compiler that this variable was not set. It will then use the default.

```javascript
myName(undefined, 'Pleek') // 'Joshua Pleek'
```
