## JavaScript Algorithms and Data Structures

An algorithm is a series of step-by-step instructions that describe how to do something.

To write an effective algorithm, it helps to break a problem down into smaller parts and think carefully about how to solve each part with code.

This repository contains JavaScript based examples that will teach you the fundamentals of algorithmic thinking by writing functions that do everything from converting temperatures to handling complex 2D arrays.

All of these examples are from FreeCodeCamp's [course](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures).

## Table of Contents

- [Basic Algorithm Scripting](#basic-algorithm-scripting)
  - [1. Convert Celsius to Fahrenheit](#1-convert-celsius-to-fahrenheit)
  - [2. Reverse a String](#2-reverse-a-string)
  - [3. Factorialize a Number](#3-factorialize-a-number)
  - [4. Find the Longest Word in a String](#4-find-the-longest-word-in-a-string)

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

### 3. Factorialize a Number

### Difficulty: Beginner

Return the factorial of the provided integer.

If the integer is represented with the letter n, a factorial is the product of all positive integers less than or equal to n.

Factorials are often represented with the shorthand notation n!

For example: 5! = 1 _ 2 _ 3 _ 4 _ 5 = 120

Only integers greater than or equal to zero will be supplied to the function.

---

### Solution 1

```
function factorialize(num) {
  if (num === 0) {
    return 1;
  } else return num * factorialize(num - 1);
}

factorialize(5);

```

### Solution 2

```
function factorialize(num) {
  let factorializedNumber = 1;
  for (let i = 2; i <= num; i++) {
    factorializedNumber *= i;
  }
  return factorializedNumber;
}

factorialize(5);


```

### 4. Find the Longest Word in a String

### Difficulty: Beginner

Return the length of the longest word in the provided sentence.

Your response should be a number.

---

### Solution 1

```
function findLongestWordLength(str) {
  let splitWords = str.split(" ");
  let longestWordLength = 0;

  for (let i = 0; i < splitWords.length; i++) {
    if (splitWords[i].length > longestWordLength) {
      longestWordLength = splitWords[i].length;
    }
  }
  return longestWordLength;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");

```
