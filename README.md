# Working with Numbers: The Math Object

## The parseInt() Function

The `parseInt()` function is used to convert a string into an integer.

### Syntax

```javascript
parseInt(string, base);
```

-   string: The string value you want to convert.
-   base: An optional base used by the number in `string`. If you omit
    this value, JavaScript uses
    <a href="https://www.twinkl.co.nz/teaching-wiki/base-10"
    target="_blank">base 10</a>.

Note that if the `string` argument contains a string representation of a
floating-point value, `parseInt()` returns only the integer portion.
Also, if the string begins with a number followed by some text,
`parseInt()` returns the number (or, at least, its integer portion). The
following table shows you the `parseInt()` results for various `string`
values.

| string   | parseInt(string) |
| -------- | ---------------- |
| "5"      | 5                |
| "5.1"    | 5                |
| "5.9"    | 5                |
| "5 feet" | 5                |
| "take 5" | NaN              |
| "five"   | NaN              |

## The parseFloat() Function

The `parseFloat()` function is similar to `parseInt()`, but you use it
to convert a string into a floating-point value:

### Syntax

```javascript
parseFloat(string);
```

Note that if `string` argument contains a string representation of an
integer value, `parseFloat()` returns just an integer. Also, like
`parseInt()`, if the string begins with a number followed by some text,
`parseFloat()` returns the number. The following table shows you the
`parseFloat()` results for some `string` values.

| string   | parseFloat(string) |
| -------- | ------------------ |
| "5"      | 5                  |
| "5.1"    | 5.1                |
| "5.9"    | 5.9                |
| "5 feet" | 5                  |
| "take 5" | NaN                |
| "five"   | NaN                |

## The `+` Operator

For quick conversions from a string to a number, most often use the +
operator, which tells JavaScript to treat a string that contains a
number as a true numeric value. For example, consider the following
code:

```javascript
const numOfShoes = "2";
const numOfSocks = 4;
const totalItems = +numOfShoes + numOfSocks;
```

By adding `+` in front of the `numOfShoes` variable, I force JavaScript
to set that variables value to the number 2, and the result of the
addition will be 6.

## The Math Object's Properties And Methods

The `Math` Object is a bit different than most of the other Objects you
come across. That's because you never create an instance of the `Math`
Object that gets stored in a variable. Instead, the `Math` Object is a
built-in JavaScript Object that you use as is. The rest of this
explores some properties and methods associated with the `Math` Object.

### Properties of the Math Object

The `Math` Object's properties are all constants that are commonly used
in mathematical operations. Table 1-1 lists all the available `Math`
Objects properties.

| Property Syntax | What it represents          | Approximate Value |
| --------------- | --------------------------- | ----------------- |
| Math.E          | Euler's constant            | 2.71828           |
| Math.LN10       | The natural logarithm of 10 | 2.30258           |
| Math.LN2        | The natural logarithm of 2  | 0.69314           |
| Math.LOG2E      | Base 2 logarithm of E       | 1.44269           |
| Math.LOG10E     | Base 10 logarithm of E      | 0.43429           |
| Math.PI         | The constant pi             | 3.14159           |
| Math.SQRT1_2    | The square root of 1/2      | 0.70710           |
| Math.SQRT2      | The square root of 2        | 1.41421           |

Table 1-1 Some Properties of the Math Object

### Methods of the Math Object

The `Math` Object's methods enable you to perform mathematical
operations such as square roots, powers, rounding, trigonometry, and
more. Many of the `Math` Object's methods are summarized in Table 1-2.

| Method Syntax              | What it Returns                                                                    |
| -------------------------- | ---------------------------------------------------------------------------------- |
| Math.abs(number)           | The absolute value of `number` (that is, the number without any sign)              |
| Math.cbrt(number)          | The cube root of `number`                                                          |
| Math.ceil(number)          | The smallest integer greater than or equal to `number` (ceil is short for ceiling) |
| Math.cos(number)           | The cosine of `number`; returned values range from -1 to 1 (input in radians)      |
| Math.exp(number)           | `E` raised to the power of `number`                                                |
| Math.floor(number)         | The largest integer less than or equal to `number`                                 |
| Math.log(number)           | The natural logarithm (base `E`) of `number`                                       |
| Math.max(number1, number2) | The largest of the provided numbers                                                |
| Math.min(number1, number2) | The smallest of the provided numbers                                               |
| Math.pow(number1, number2) | `number1` raised to the power of `number2`                                         |
| Math.random()              | A random number between 0 (inclusive) and 1 (exclusive)                            |
| Math.round(number)         | The integer closest to `number`                                                    |
| Math.sin(number)           | The sine of `number`; returned values range from -1 to 1 (input in radians)        |
| Math.sqrt(number)          | The square root of `number` (which must be greater than or equal to 0)             |
| Math.tan(number)           | The tangent of `number` (input in radians)                                         |
| Math.trunc(number)         | The integer portion of `number`                                                    |

Table 1-2 Some Methods of the Math Object
