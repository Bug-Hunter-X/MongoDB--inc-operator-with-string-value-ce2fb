# MongoDB $inc operator with string value
This repository demonstrates an uncommon error related to the usage of the `$inc` operator in MongoDB update operations. Specifically, it showcases the issue of providing a string value instead of a numeric value to the `$inc` operator, leading to unexpected behavior or errors.

## Bug Description
The `$inc` operator is designed to increment a numeric field by a specified value. However, if you provide a string value as the increment, the operation will not perform as expected.  This can be difficult to detect as MongoDB might not raise an immediate error.

## Solution
Always ensure that the value provided to the `$inc` operator is a valid number (integer or float).