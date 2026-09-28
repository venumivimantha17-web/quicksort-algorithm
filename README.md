# Quicksort Algorithm

A Python implementation of the **Quicksort algorithm** using recursion and partitioning.

## 📌 Overview

Quicksort is a divide-and-conquer sorting algorithm that organizes elements by selecting a **pivot** and partitioning the remaining elements into smaller and larger groups.

This implementation uses the **first element of the list as the pivot** and divides the input into three sublists:

* **Less** — elements smaller than the pivot
* **Equal** — elements equal to the pivot
* **Greater** — elements greater than the pivot

The sublists are then recursively sorted and combined to produce the final sorted list.

## Features

* Implements Quicksort using recursion
* Uses the first element as the pivot
* Handles duplicate values correctly
* Returns a new sorted list
* Does not modify the original input list
* Does not use Python's built-in sorting functions
* Requires no external modules

## Algorithm

1. If the list contains zero or one element, return a copy of the list.
2. Select the first element as the pivot.
3. Create three sublists:

   * Elements less than the pivot
   * Elements equal to the pivot
   * Elements greater than the pivot
4. Recursively apply Quicksort to the less and greater sublists.
5. Concatenate the sorted sublists with the equal elements.
6. Return the final sorted list.

## Example

```python
from quick_sort import quick_sort

numbers = [20, 3, 14, 1, 5]

result = quick_sort(numbers)

print(result)
```

Output:

```text
[1, 3, 5, 14, 20]
```

The original list remains unchanged:

```python
numbers = [20, 3, 14, 1, 5]

result = quick_sort(numbers)

print(numbers)
print(result)
```

Output:

```text
[20, 3, 14, 1, 5]
[1, 3, 5, 14, 20]
```

## 🧪 Duplicate Values

The algorithm correctly handles duplicate values.

```python
numbers = [87, 11, 23, 18, 18, 23, 11, 56, 87, 56]

print(quick_sort(numbers))
```

Output:

```text
[11, 11, 18, 18, 23, 23, 56, 56, 87, 87]
```

## 📂 Project Structure

```text
quicksort-algorithm/
│
├── quick_sort.py
└── README.md
```

## ⚙️ Requirements

* Python 3.x
* No external dependencies

## 📚 Concepts Demonstrated

* Recursion
* Divide-and-conquer algorithms
* List manipulation
* Algorithmic problem solving
* Time and space complexity concepts

## 📄 License

This project is created for educational and learning purposes.
