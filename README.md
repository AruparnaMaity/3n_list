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