# MongoDB $inc operator error with string value
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The error occurs when a string value is used instead of a numeric value for the increment amount.

## Bug Description
The `$inc` operator is used to increment a numeric field in a MongoDB document.  If you attempt to increment a field using a string, the operation will likely fail, or unexpectedly modify the field by assigning the string rather than incrementing it.

## Solution
Ensure that you are providing a valid numeric value to the `$inc` operator. This will increment the field correctly.

## How to reproduce the bug
1. Clone this repository.
2. Make sure you have MongoDB and a driver of your choice installed and running
3. Run the script `bug.js` to execute the query with incorrect usage of `$inc` operator.
4. Run the script `bugSolution.js` to see the correct usage of `$inc` operator