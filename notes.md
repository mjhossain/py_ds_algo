## Big-O Introduction
Big-O is used to measure code execution efficency using time complexity and space complexity. 
**Time complexity** uses number of operations to measure 2 algorithm/code execution.
**Space complexity** uses amout of memory it takes during code/algorithm execution.
Space complexity has more priority then time complexity when it comes to Big-O.

### Big-O Cases
**Best Case** is an Omega
**Avg Case** is Beta
**Worst Case** is O

**Big-O is always used to calculate the worst case**


![Big-O Complexity Chart](o-complexity.png)
Big-O Complexity Chart

## O(n) || Big-O of n
O(n) takes *n* number of operations to complete execution.

O(n) code sample
```
def print_items(n):
    for i in range(n):
        print(i)
  
# DO NOT CHANGE THIS LINE:
print_items(10)
```