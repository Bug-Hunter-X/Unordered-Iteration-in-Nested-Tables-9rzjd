# Unordered Iteration in Nested Tables in Lua

This repository demonstrates an uncommon bug in Lua related to the unordered iteration of nested tables using `pairs`.  The `pairs` iterator does not guarantee any specific order of iteration, which can lead to unexpected results when processing nested data structures.

The `bug.lua` file shows a recursive function that attempts to process a nested table. Due to the unordered nature of `pairs`, the output might not be consistent across different Lua implementations or runs.

The `bugSolution.lua` file offers a solution demonstrating how to maintain a consistent order using a sorted table.