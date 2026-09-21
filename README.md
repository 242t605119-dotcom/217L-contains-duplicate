# LeetCode 217 - Contains Duplicate

## Problem Description

Given an integer array `nums`, determine whether any value appears at least twice in the array.

Return `True` if a duplicate exists. Otherwise, return `False`.

## Example

Input:

nums = [1,2,3,1]

The number `1` appears more than once.

Output:

True

Another example:

nums = [1,2,3,4]

All elements are different.

Output:

False

## Approach

We use a **set** to keep track of the numbers that have already been seen.

While traversing the array, we check whether the current number is already present in the set.

If it is already present, a duplicate exists, so we return `True`.

Otherwise, we add the number to the set and continue.

If the complete array is processed without finding a duplicate, we return `False`.

## Algorithm

1. Create an empty set called `seen`.
2. Traverse every number in the array.
3. Check whether the number is already in `seen`.
4. If it exists, return `True`.
5. Otherwise, add it to the set.
6. Return `False` if no duplicate is found.

## Time Complexity

**O(n)**

Each element is checked and added to the set at most once.

## Space Complexity

**O(n)**

In the worst case, the set stores all elements of the array.

## Key Concepts

- Set
- Arrays
- Duplicate Detection
- Hashing
- Traversal

## Author

T.nandhini
