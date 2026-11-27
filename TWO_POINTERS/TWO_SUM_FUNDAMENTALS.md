'''TWO SUM ---> INTERNAL UNDERST

Let's use your exact example and physically eliminate the possibilities.
arr = [2, 5, 7, 12, 13, 15, 16]
target = 12



Step 1: Imagine all possible pairs
Initially, your pointers are at 2 and 16.
LEFT → 2
16 ← RIGHT

2 + 16 = 18
Too large!

Your instinct might be:

"Why should I move the right pointer? What if the correct answer is 5 + 7?"

Excellent question.
Step 2: Let's prove why moving right is safe or why should we eliminate 16 
Because the array is sorted:
2, 5, 7, 12, 13, 15, 16

Look at every possible pair involving 16:
Pair	Sum
2 + 16	18
5 + 16	21
7 + 16	23
12 + 16	28
13 + 16	29
15 + 16	31

All impossible
Why?

Because even the smallest number, 2, produces a sum greater than 12 when paired with 16.

Therefore, 16 cannot be part of the answer with any other element.

We can safely eliminate it.
Step 3: Move right pointer
LEFT → 2
15 ← RIGHT

2 + 15 = 17
Too large!
Again, even 2 + 15 is greater than 12. So 15 cannot be part of the answer either.

Continue:
Left	Right	Sum	Action
2	16	18	Remove 16
2	15	17	Remove 15
2	13	15	Remove 13
2	12	14	Remove 12
2	7	9	Remove 2
5	7	12	Found!

Look what happened!

We didn't skip (5, 7).

We safely eliminated numbers that mathematically could not participate in a valid pair.'''