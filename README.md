# JavaScript Function NaN Handling Bug

This repository demonstrates a subtle bug in a JavaScript function that handles null, negative numbers, and positive numbers correctly, but unexpectedly returns NaN instead of a specific value when given NaN as input.

## Bug Description

The `foo` function is designed to handle null, negative, and positive numeric values, but it does not properly handle NaN (Not a Number).  Instead of returning a specific value or throwing an error, it simply returns NaN. This behavior may be unexpected and lead to errors if NaN is an expected input.

## Solution

The solution addresses this issue by explicitly checking for `isNaN(x)` and returning a predefined value or throwing an error based on how NaN should be handled in the specific context.