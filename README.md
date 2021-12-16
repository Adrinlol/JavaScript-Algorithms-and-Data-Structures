## JavaScript Algorithms and Data Structures

An algorithm is a series of step-by-step instructions that describe how to do something.

To write an effective algorithm, it helps to break a problem down into smaller parts and think carefully about how to solve each part with code.

This repository contains JavaScript based examples that will teach you the fundamentals of algorithmic thinking by writing functions that do everything from converting temperatures to handling complex 2D arrays.

All of these examples are from FreeCodeCamp's [course](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures).

## Table of Contents

- [Basic Algorithm Scripting](#basic-algorithm-scripting)
  - [1. Convert Celsius to Fahrenheit](#1-convert-celsius-to-fahrenheit)
  - [2. Reverse a String](#2-reverse-a-tring)

## Basic Algorithm Scripting

### 1. Convert Celsius to Fahrenheit

### Difficulty: Beginner

The algorithm to convert from Celsius to Fahrenheit is the temperature in Celsius times 9/5, plus 32.

You are given a variable celsius representing a temperature in Celsius. Use the variable fahrenheit already defined and assign it the Fahrenheit temperature equivalent to the given Celsius temperature. Use the algorithm mentioned above to help convert the Celsius temperature to Fahrenheit.

---

### Solution

```
function convertToF(celsius) {
  let fahrenheit = (celsius * 9) / 5 + 32;
  return fahrenheit;
}

convertToF(30);
```

### 2. Reverse a String

### Difficulty: Beginner

Reverse the provided string.

You may need to turn the string into an array before you can reverse it.

Your result must be a string.

---

### Solution 1

```
function reverseString(str) {
  return str.split("").reverse().join("");
}

reverseString("hello");
```

### Solution 2

```
function reverseString(str) {
  let reversedString = "";
  for (let i = str.length - 1; i >= 0; i--) {
    reversedString += str[i];
  }
  return reversedString;
}

reverseString("hello");

```
