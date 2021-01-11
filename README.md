# 3-n List

## Explanation of the problem

In the 3- list problem you will be provided with a list of length 3 times of a positive integer. You have to create triplets from the elements of that list in such a way that the sum of the middle elements is the largest but the first element is smaller than the second and the third element is larger than the second.

## Example

Consider the following list of integers.

```python
list_3n = [2, 3, 10, 7, 5, 3]
```

The above list is of length 6. Thus we would be able to create a list of 2 triplets, and the correct result should be:

```python
[(2, 7, 10), (3, 3, 5)]
```

[(3, 10, 7), (2, 5, 3)] is not a correct result.

## Solution

**Step 1:** First sort the input list in ascending order

```python
list_3n_sorted = list_3n.sort()
```

**Step 2:** Get the following 3 elements from the sorted list:
1. First element from the sorted list
```python
list_3n_sorted[0]
```

2. Second last element from the sorted list
```python
list_3n_sorted[-2]
```

3. Last element from the sorted list
```python
list_3n_sorted[-1]
```

**Step 3:** Slice the sorted list leaving the above 3 elements out.
```python
list_3n_sorted = list_3n_sorted[1:-2]
```

**Step 4:** Repeat Step 2 and Step 3 until the length of `list_3n_sorted` becomes 0, then break the while loop.