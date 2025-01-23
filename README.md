# JavaScript Falsy Value Handling Bug

This repository demonstrates a common, yet subtle bug in JavaScript related to handling falsy values within a function designed to perform addition.

## Bug Description
The `foo` function is designed to add two numbers. It explicitly handles `null` values, returning 0 if either input is null. However, it doesn't account for other falsy values such as `0`, `false`, `undefined`, or an empty string.  This can lead to unexpected results.

## Bug Solution
The solution improves the function's handling of falsy values. We use explicit checks to ensure both inputs are numbers before performing the addition.