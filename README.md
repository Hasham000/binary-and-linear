# Search Algorithms: Linear and Binary Search

This repository provides Python implementations of two classic search algorithms: **Linear Search** and **Binary Search**. These algorithms are used to find the position of a target element within a given list.

## Features

- **Linear Search:** A simple algorithm that checks each element of the list sequentially.
- **Binary Search:** A more efficient algorithm that works on sorted lists by repeatedly dividing the search interval in half.

## Functions

### `linear_search(arr, target)`
Searches for the `target` element in the list `arr` using the linear search method.

#### Parameters:
- `arr` (list): The list to search through.
- `target` (int, float, etc.): The element to find in the list.

#### Returns:
- Index of the `target` element if found.
- `-1` if the `target` element is not in the list.

### `binary_search(arr, target)`
Searches for the `target` element in the sorted list `arr` using binary search.

#### Parameters:
- `arr` (list): The sorted list to search through.
- `target` (int, float, etc.): The element to find in the list.

#### Returns:
- Index of the `target` element if found.
- `-1` if the `target` element is not in the list.

## Usage Example

```python
arr = [2, 3, 4, 10, 40]
target = 10

# Linear Search
print("Linear Search:")
result = linear_search(arr, target)
if result != -1:
    print(f"Element found at index {result}")
else:
    print("Element not found")

# Binary Search
print("\nBinary Search:")
arr.sort()  # Make sure the array is sorted for binary search
result = binary_search(arr, target)
if result != -1:
    print(f"Element found at index {result}")
else:
    print("Element not found")
```

### Output:

```
Linear Search:
Element found at index 3

Binary Search:
Element found at index 3
```

## Worst-Case for Binary Search

If searching in an array of size n = 8:
 
[1, 3, 5, 7, 9, 11, 13, 15] 
Target: 2 (not in the list)
Binary search will go through:
 
Midpoint: 7
Midpoint: 3
Midpoint: 1
Not found.
Total comparisons: log_2(8) = 3, showing O(log n) complexity.
 
## Prerequisites

- Python 3.x

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/search-algorithms.git
   cd search-algorithms
   ```

2. Run the Python script:
   ```bash
   python search_algorithms.py
   ```

## linked in post link

https://www.linkedin.com/posts/hasham-ali-noor-151672347_github-hasham000binary-and-linear-activity-7286698102218997760-SVe_?utm_source=share&utm_medium=member_ios



## License

This project is licensed under the MIT License

---

Feel free to contribute to this project or improve the algorithms. If you have any questions or issues, open an issue or create a pull request!
