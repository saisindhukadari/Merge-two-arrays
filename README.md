# Merge-two-arrays

## Problem Statement

Given two arrays `arr1` and `arr2` of sizes `n` and `m`, merge them into a single array containing all elements of both arrays.

Unlike the union operation, **merging simply concatenates the arrays** without removing duplicate elements.

---

## Approach

1. Read the sizes of both arrays.
2. Read the elements of each array.
3. Create a new array of size `n + m`.
4. Copy all elements of the first array into the new array.
5. Copy all elements of the second array after the last element of the first array.
6. Print the merged array.

---

## Algorithm

1. Input `n` and `m`.
2. Create two arrays:

   * `arr1` of size `n`
   * `arr2` of size `m`
3. Read the elements of both arrays.
4. Create a new array `merged` of size `n + m`.
5. Copy `arr1` into `merged`.
6. Copy `arr2` into the remaining positions of `merged`.
7. Display the merged array.

---

## Example

### Input

```text
3 3
1 2 3
4 5 6
```

### Output

```text
[1, 2, 3, 4, 5, 6]
```

---

## Time Complexity

* **O(n + m)**

Each element from both arrays is copied exactly once.

---

## Space Complexity

* **O(n + m)**

An additional array is created to store the merged result.

---

## Concepts Used

* Arrays
* Array Traversal
* Copying Elements
* Java `Arrays.toString()`

---

## Notes

* This program **does not sort** the merged array.
* Duplicate elements are preserved.
* The relative order of elements from each input array remains unchanged.

### Example with Duplicates

#### Input

```text
3 3
1 2 2
2 3 4
```

#### Output

```text
[1, 2, 2, 2, 3, 4]
```

The program simply appends the second array after the first without removing duplicates.
