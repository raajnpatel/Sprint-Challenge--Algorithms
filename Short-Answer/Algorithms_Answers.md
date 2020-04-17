#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)

for every additional unit in the input 'n', the runtime increases by that number.

a < 1 * 1 * 1 = a < 1 a = a+1 runs once a< 2 * 2 * 2 = a < 8 a = a+4 runs twice, etc.

b) O(n log n) the initial for loop is a straight O(n) runtime, because it runs for every number in a given input range. There is a nested while loop that runs while j < n. j gets multiplied by 2 each time, halving the total amount of iterations, leading me to O(log n)

if n is 3, the first for loop will run 3 times,
each time, the while loop will run 3 times (j = 1, j =2 , j= 4, break)

if n is 5, the first for loop will run 5 times,
the while loop will run 4 times. (j=1, j=2, j=4, j=8, break)

if n is 7, the first for loop will run 7 times,
the while loop will run 4 times (j=1, j=2, j=4, j=8, break)

Since the while loop grows lower than the proportional increase in the input size, we assume O(log n) for that part.

c) O(n) The function will run a number of times equal to the amount given in 'bunnies', therefore it is O(n) n equals the amount of bunnies passed in.

## Exercise II

get halfway_point = n // 2

Test to see if egg breaks at halfway_point.

if egg breaks, take lower half of the array, find halfway point and repeat

if egg doesn't break, take upper half of array, find halfway point and repeat.

repeat process until you move in one direction by one spot. If the egg breaks, and you move one spot down and the egg doesn't break.. The previous spot is 'f'.

if the egg doesn't break and you move up one and it does break, that last one is your 'f'

Since we are halving every time, the runtime complexity would be O(log n)

n would represent the amount of floors