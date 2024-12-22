# Incorrect Usage of $inc Operator in MongoDB Update Operation
This example demonstrates an error that can occur when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field by a specified value.  However, if a string is provided as the increment value, MongoDB will throw an error.

## Bug
The bug lies in the incorrect usage of the `$inc` operator. The code attempts to increment the `counter` field by the string value '1'. This is not allowed, as the `$inc` operator requires a numeric value. 

## Solution
The solution is to ensure that the increment value is a number (integer or float).  The corrected code uses the number 1 instead of the string '1'.