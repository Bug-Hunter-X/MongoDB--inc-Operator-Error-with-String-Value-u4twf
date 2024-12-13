# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error occurs when attempting to increment a field whose value is a string instead of a number.

## Bug Description
The bug is caused by incorrectly passing a string value to the `$inc` operator.  The `$inc` operator expects a numerical value to increment.  Passing a string results in an error.

## Solution
The solution involves ensuring that the field being incremented is of numerical type.  If the field needs to be initialized, it should be initialized with a number. The updated code should use a number in the $inc operation. 
