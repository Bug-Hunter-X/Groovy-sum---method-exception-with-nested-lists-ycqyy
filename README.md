# Groovy Nested List Sum Bug

This repository demonstrates a common issue when using the `sum()` method in Groovy with nested lists.  The `sum()` method, when applied to a list of lists, throws an exception instead of recursively summing the elements.  The solution provided shows how to correctly handle this scenario.

## Bug Description
The `sum()` method in Groovy works perfectly fine for a flat list of numbers. However, when applied to a nested list (a list of lists), it throws a `groovy.lang.MissingMethodException`. This is because `sum()` expects numerical values, and a list is not a number.  The solution shows how to flatten the nested list first before performing the sum operation.

## Solution
The solution utilizes the `flatten()` method to convert the nested list into a single list of numbers, which `sum()` can then successfully operate on.