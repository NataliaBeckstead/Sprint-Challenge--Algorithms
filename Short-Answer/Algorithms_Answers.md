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

b) O(n^2)

2 nested loops, both depends on n

c) O(n)

function will be executed as many times, as many bunnies we have
same time complecsity as a loop, but taking more memory

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

start at floor f
while we have space to throw egg
    throw egg
at this moment we're out of eggs, or all floors below f+1 full of eggs
also we haven't broke as many eggs as we can
all other eggs will be broken
while we still have eggs
    floor += 1
    throw all eggs this floor can fit

Since number of iterations depends on amount of eggs, time complexity will be O(n)
