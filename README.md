## Big-O Introduction
Big-O is used to measure code execution efficency using time complexity and space complexity. 
**Time complexity** uses number of operations to measure 2 algorithm/code execution.
**Space complexity** uses amout of memory it takes during code/algorithm execution.
Space complexity has more priority then time complexity when it comes to Big-O.

### Big-O Cases
**Best Case** is an Omega ($\Omega$)
**Avg Case** is Big Thetha ($\theta$)
**Worst Case** is O 

**Big-O is always used to calculate the worst case**


#### Drop Constats
In order to simplify O(n) we can drop any constant before n. Example O(2n) would be written as O(n).

#### Drop Non-Dominants
In an algorthim if there are multiple operations and the algorithm looks like O(n^3 + n) then the non-dominant operation in this case n will be dropped and rewritten as O(n^3) instead of O(n^3 + n).

#### Big-O Terminology
O(1) : Constant
O(n) : Propotional
O(log n) : Divide & Conquer
O(n^2) : Loop within a loop 


![Big-O Complexity Chart](o-complexity.png)
Big-O Complexity Chart

![Big-O Complexity Chart](<Screenshot 2023-10-03 at 12.44.27 AM.png>)
<hr />

#### O(n) || O of n
O(n) takes *n* number of operations to complete execution.

O(n) code sample
```python
def print_items(n):
    for i in range(n):
        print(i)
  
# DO NOT CHANGE THIS LINE:
print_items(10)
```



#### O(n^2) || O of n square
O(n^2) take *n\*n* number of operations to complete execution.

O(n^2) code example
```python
def print_items(n):
    for i in range(n):
        for j in range(n):
            print(i,j)

print_items(10)
```


code example:
```python
def print_items(n):
    for i in range(n):
        for j in range(n):
            print(i,j)
    
    for k in range(n):
        print(k)

print_items(10)
```


#### O(1) || O of 1 || Constant
An O(1) takes just 1 operation to complete. Sometimes reffered to as constant.

code example:
```python
def add_item(n):
    return n+n

print(add_item(10))
```


#### O(log n) || O of log n
If used in an already sorted list,  O(log n) is one of the most efficent algorithm. 
**2^3 = 8** can be written as **log<sub>2</sub> 8 = 3**


#### Different Terms of Inputs
When an algorithm has 2 different inputs it is considered as *different terms of inputs*.

Example 1:
```python
def print_items(a, b):
    for i in range(a):
        print(i)

    for j in range(b):
        print(j)

print_items(2, 4)
```
The avobe code would be written as O(a) + O(b) or simply **O(a + b)**


Example 2:
```python
def print_items(a, b):
    for i in range(a):
        for j in range(b):
            print(i, j)
    

print_items(2, 4)
```
The avobe code would be written as O(a) * O(b) or simply **O(a * b)**

<hr />

#### Big-O of Lists in Python
Inserting/Removing at the beginning of a list is O(n) as we re-assign the indexes
Inserting/Removing at the end of a list is O(1)
Inserting/Removing at the middle of a list is O(n) as we re-assign the indexes
Searching by value is O(n)
Searching by index is O(1)









<hr />
#### External Resources
[Big-O Cheatsheet](https://www.bigocheatsheet.com/)