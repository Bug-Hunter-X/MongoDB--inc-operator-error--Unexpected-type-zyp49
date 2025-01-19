# MongoDB $inc operator error: Unexpected type
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical field by a specified value.  However, if the specified value is not a number, an error will occur.  This example shows the incorrect usage and the correct solution.

## Bug
The bug lies in the incorrect use of the `$inc` operator. The value being incremented should always be a number.  In the buggy code, we're attempting to increment the `count` field by the string '1'.

## Solution
The solution is to ensure that the value passed to the `$inc` operator is a number.  This ensures that the MongoDB update operation executes correctly, incrementing the `count` field by 1.
