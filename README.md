# Working with Numbers: The Math Object

This guide provides an overview of using JavaScript's built-in functions and methods for working with numbers, focusing on `parseInt()`, `parseFloat()`, the `+` operator, and the `Math` object's properties and methods.

## The parseInt() Function

The `parseInt()` function is used to convert a string into an integer.

### Syntax

```javascript
parseInt(string, base);
```

1. _string_: The string value you want to convert.
2. _base_: An optional base used by the number in string. If you omit this value, JavaScript uses base 10.

Note that if the string argument contains a string representation of a floating-point value, parseInt() returns only the integer portion. Also, if the string begins with a number followed by some text, parseInt() returns the number (or, at least, its integer portion). The following table shows you the parseInt() results for various string values.

| string   | parseInt(string) |
| -------- | ---------------- |
| "5"      | 5                |
| "5.1"    | 5                |
| "5.9"    | 5                |
| "5 feet" | 5                |
| "take 5" | NaN              |
| "five"   | NaN              |

## The parseFloat() Function

The `parseFloat()` function is similar to `parseInt()`, but you use it to convert a string into a floating-point value:

### Syntax

```javascript
parseFloat(string);
```

Note that if `string` argument contains a string representation of an integer value, `parseFloat()` returns just an integer. Also, like `parseInt()`, if the string begins with a number followed by some text, `parseFloat()` returns the number. The following table shows you the `parseFloat()` results for some `string` values.

| string   | parseFloat(string) |
| -------- | ------------------ |
| "5"      | 5                  |
| "5.1"    | 5.1                |
| "5.9"    | 5.9                |
| "5 feet" | 5.2                |
| "take 5" | NaN                |
| "five"   | NaN                |
