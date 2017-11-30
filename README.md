# Javascript Values Types and operators

In this section we will go over the very basics and building blocks of Javascript. This challenge will cover the lessons learned from Chapter 1 of the Eloquent Javascript Book [link](http://eloquentjavascript.net/01_values.html). I recommend you to go ahead an read through the chapter yourself, but this tutorial will give you the bare essentials.

## Everything is a bit
If you every seen the matrix, you have seen what binary looks like. A bunch of zeros and ones. something like this `01000101`.
Per the book, any piece of discrete information can be reduced to a sequence of zeros and ones and thus represented in bits.

## Six Basic Types of Values in Javascript

There are six basic types in javascript: Numbers, Strings, Booleans, Objects, Functions, and Undefined values.
For now we will go over Numbers, Strings, Boolean, and Undefined Values for this chapter.

### Numbers

A number is exactly what it sounds like. a number :) for example 7.
However, there are few things you need to be aware of for programming in Javascript

In Javascript there is a limit to how large and precise a number can be. This number is very large, but it is something you should be aware of. The max safe Integer is 9007199254740991. FYI a Integer is another world for whole numbers. Also for float numbers, e.a. decimal numbers, Javascript has a limit to how many decimal places it can store.

You won't have to deal with such large and precise numbers often, but just remember that there are these limitations

Another tidbit in Javascript is NaN. NaN stands for Not a Number, and it is used when something nonsensical value is described. infinity or -infinity. You will see NaN when you try to divide by zero.

### Arithmetic

Javascript supports basic math operators such as `+ - * /` it also follows the order of operations. When in doubt put parentheses around your math. There is also another operator called modulo `%`, which is just a fancy name for remainder

### Strings
In Javascript you define a string by putting `" quotes around it "` it can be singles quotes as well. You can also add a backslash, `\`, to escape the character and add special characters like next line. `Hello \n`. The `\` escapes the character and the `n` is a symbol to create a new line.

### Boolean Values
In Javascript boolean values are just true or false. It is used when you only need to check between two options.

#### Comparison
When you perform comparisons in Javascript you will return a boolean value.
In Javascript there are 8 comparison operators.

- `==`:equal to
- `===`: equal value and equal types
- `!=`: not equal
- `!==`: not equal value or not equal type
- `>`: greater than
- `<`: less than
- `>=`: greater than or equal to
- `<=`: less than or equal to

So if you compare 3 > 2 Javascript would return `true`.

NOTE: In regards to `==` vs `===` and `!=` vs `===` we will get into what data types are, but for now just defensively use `===` and `!==`.

You might wonder what would happen if you compare something other than numbers. Javascript follows the [Unicode Standard](https://unicode-table.com/en/) and all characters in a string is compared like a number based on their position in the unicode.

For Example `b < a` would return `false`

#### Logical Operators

There are three logical operators
- `&&`: and operator requires both values to be true
- `||`: or operator requires one value to be true
- `!`: not operator flips the value

For example:
- `true && true = true`
- `true || false = true`
- `!false = true`

### Undefined values
In Javascript there is two undefined values.

- `null`
- `undefined`

They both denote the absence of value.

### Automatic type conversion

Javascript was original meant for beginners, and because of that Javascript has Automatic type conversion. You will learn all about types in Javascript, but they are essentially a representation of what the value should be. For example for numbers there are Integers and Floats. Theses two are data types. Integers are whole numbers and Floats are decimal numbers. For now just understand that javascript automatic converts types for you so watch out for them.

NOTE: you can see the type of a value by using the unary operator `typeof`. For example  `typeof 13` will output as `Integer`

## Challenge

For this challenge you will need to create a javascript file and log a few things to the console.

HINT: `console.log(value)` and where `value` is what you want to long.

1. log a Integer number
2. log a Float number
3. log a string
4. log a string with the `\` character in it
5. log a comparison between two numbers
5. log a comparison between two strings
6. log a logical operator
7. log the data type of a number and string
