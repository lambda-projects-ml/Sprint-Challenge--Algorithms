## Exercise I

a. O(n) - Loops through the while loop `n` times until the boolean condition is met

b. O(n^3) - the first three for loops have a range dependent on `n`. The last loop has a static range of 10

c. O(n) - the function is being called recursively `n` times before reaching the base case

## Exercise II

Similar to a binary search. Need to find where the floor next to it is different.

number of floors = 20

Time complexity : O(log n)

```
    Check middle floor (10) for breaking egg
        if egg breaks discard lower half of floors (each floor an egg breaks on append it to a list)
            select middle floor of upper half (15)
                if egg breaks check floors below(11 - 14)
                else check floors above(16-20)
        else check lower half and discard upper floors
            select middle floor of lower half (5)
                if egg breaks check floors below(1 - 14)
                else check floors above(6-10)

    Once all checks done return the lowest number in the list to find the lowest floor an egg will break on.
```
