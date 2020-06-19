# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```


```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.


O(log n) A binary search would be a good solution because n stories can be a large number. (Suppose that you have an n-story building and plenty of eggs.)

You would need to loop through to a middle value floor to find f first, eliminating the higher values first


Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

So you would keep cutting the targets in half till you find one that is # true thus eliminating all above it, then again eliminating more till you find the # target (Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f.)
