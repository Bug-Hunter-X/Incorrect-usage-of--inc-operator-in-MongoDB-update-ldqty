# Incorrect usage of $inc operator in MongoDB update

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numeric field by a specified value. However, in the provided example, we are attempting to increment the `age` field by a string value ('1'), which results in an unexpected behavior.

## Bug Description
The code demonstrates an incorrect usage of the $inc operator in a MongoDB update operation. The age value is being incremented by a string instead of a number, leading to unexpected results.

## Solution
The solution involves using a numeric value instead of a string value to increment the age field.

## How to reproduce the bug
1.  Set up MongoDB.
2.  Create a collection named `myCollection` with a document containing a field named `age`.
3.  Run the buggy code from `bug.js`.
4.  Observe the unexpected result.

## How to fix the bug
1.  Modify the code to use a numeric value for incrementing `age`, as in `bugSolution.js`.
2.  Run the updated code and verify the correct results.
