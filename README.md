# Nearby elements

## Story

## What are you going to learn?

You'll have to:

- work in a new programming language
- get accustomed to a new IDE
- use arrays, data structures with a pre-defined size
- avoid exceptions
- use assertions

## Tasks


1. The `NearbyElementsChecker` class is initialized with an array. Implement the `getNearbyElements` method that looks for a given target at position `(row, col)` in that array and picks its nearby elements, the ones that surround the target within a given range. The target element itself should be omitted. Might the target position fall outside of the given (existing) row, you still need to pick up the elements within its "virtual" range. Target positions with out-of-bounds `row` number should return `null`. Example: for the array `[[10, 11, 12], [20, 21, 22, 23]]`, the nearby elements within a `range` of `2` for the target at `(1, 2)` (which is `22`) would be `[20, 21, 23]`. The similar result for the off-the-edge position `(1, -1)` would be `[20, 21]`, while the result for `(5, 3)` would be `null`.

    - The target element is never included in the result array.
    - When the target element and its range is within the limits of the row, the numbers within the range are returned.
    - When the target element is within the limits of the row, but its `range`-sized neighborhood not, the returned array is shorter accordingly.
    - When the target element is outside the limits of the row but is virtual neighborhood within the distance of `range` is overlapping with the array, the intersection is returned.
    - When the target element and its `range`-sized neighborhood are outside the limits of the row, an array of length `0` is returned.
    - When the target `row` number is not found in the array, `null` is returned.

2. Implement the `prettyPrint()` method in `NearbyElementsChecker` that prints the array with numbers in the same column aligned together. Align numbers to the right. The width of each column in the table should be one character longer than the longest element in the array. Watch out: the length of a number includes its sign. Example: the result for array `[[1, 1111, 11], [2, 22, -22, 22]]` should have a column width of 5 and return `"....1.1111...11\n....2...22..-22...22"` (here `.` stands for a space).

    - The numbers in the array are all printed.
    - The width of every column is determined by the globally longest element.
    - The numbers are space-separated and aligned to the right.


## General requirements


None

## Hints

- Check the included assertions (expressions required to hold in a correct
  implementation) that test for the expected results for different arguments.
- In Java, assertions are disabled by default. You have to enable them
  by starting the JVM with the `-ea` or `-enableassertions` option.
  You can instruct your IDE to run the code with this option.
  In IntelliJ IDEA check `Run/Edit configurations...` and add the options
  to the VM Options box.
- Always perform index validation when accessing array elements
  otherwise you might run into an `ArrayIndexOutOfBounds` exception.

## Starting repository

Follow [this link](https://journey.code.cool/v2/project/solo/blueprint/nearby-elements/java) to create your project repository.

## Background materials

- :exclamation: [Arrays](https://learn.code.cool/full-stack/#/../pages/java/arrays)
- [Code style](https://learn.code.cool/full-stack/#/../pages/java/code-style)
- [Creating objects](https://learn.code.cool/full-stack/#/../pages/java/creating-objects)
- [Methods](https://learn.code.cool/full-stack/#/../pages/java/methods)
- [Running application](https://learn.code.cool/full-stack/#/../pages/java/running-application)
