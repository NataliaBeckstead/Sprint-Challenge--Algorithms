#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)

While loop is O(n^3), but step for increasing a is n^2, this way we're getting linear dependency from value of n
0 < n * n * n
   a = n * n
n * n < n * n * n
   a = 2 * n * n
2 * n * n < n * n * n
   a = 3 * n * n
3 * n * n < n * n * n
   a = 4 * n * n
etc until we run loop n times

b) O(n*log n)

2 nested loops, n and log n

c) O(n)

function will be executed as many times, as many bunnies we have
same time complecsity as a loop, but taking more memory

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

For this task I would use binary search
if in the middle of the building egg is broken, go lower for amount of floors below me / 2
if egg saved, go higher for amount of floors higher me / 2
I found f floor when I had to go up or down just 1 floor, and it will be the floor where egg didn't broke

Runtime complexity is O(log n)