Pattern 1: Two Pointers

1. What is the Two Pointers pattern?
Two Pointers means using two variables (pointers) to keep track of positions in an array, string, or linked list.

Instead of using nested loops to compare every possible pair, we use two pointers to solve the problem more efficiently.

For example:
arr = [1, 2, 3, 4, 5]left = 0right = len(arr) - 1


Here:
- left points to the first element.
- right points to the last element.
Two pointers visualization
Opposite direction


There are three important variations of Two Pointers:
1. Opposite-direction pointers.
2. Same-direction pointers.
3. Fast and Slow pointers.
We'll understand each separately.

2. When to use Two Pointers
Use case 1: Find a pair whose sum equals a target
Very frequently asked
When to use:
- You have a sorted array.
- You need to find two numbers whose sum equals a target.
- You want to avoid checking every possible pair using nested loops.