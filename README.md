# Unexpected Behavior of removeIf on Mutable Collections in Kotlin

This repository demonstrates a subtle but important issue when using the `removeIf` function on mutable collections (like `MutableList` and `MutableSet`) in Kotlin.  The problem arises from modifying the collection while iterating over it, potentially leading to unexpected results or exceptions.

The `BugRemoveIf.kt` file shows how `removeIf` might not remove all intended elements because the indices are changing during the iteration process.

The `SolutionRemoveIf.kt` file provides solutions, illustrating safe ways to modify mutable collections during iteration.