# Type Coercion Bug in JavaScript Addition Function

This repository demonstrates a subtle bug related to type coercion in a simple JavaScript addition function. The function `foo` is intended to add two numbers, but it incorrectly handles cases where one or both inputs are 0, treating them as null.

## Bug Description

The issue stems from the use of strict equality (`===`) in the conditional statement.  When a number is passed as 'a' or 'b' which is loosely equal to null (0), the condition evaluates to true and the function returns null.

## Solution

The solution involves modifying the conditional check to explicitly handle 0 values separately from null values using loose equality.