Binary Search Implementation in Java

Binary Search is a widely used search algorithm that finds the position of a target element within a sorted array. It operates by dividing the search interval in half repeatedly, reducing the search space to logarithmic time complexity.


---

✨ Key Concepts

What is Binary Search?

Binary Search is an efficient algorithm to locate a target element in a sorted array.

It compares the target with the middle element and eliminates half of the search space based on the comparison result.


Why Use Binary Search?

Efficiency: Time complexity of O(log n), making it much faster than linear search for large datasets.

Requirements: The array must be sorted beforehand.



---

🔍 How It Works

1. Initialize: Start with two pointers, low and high, representing the beginning and end of the array.


2. Find Midpoint: Calculate the middle index:

int mid = low + (high - low) / 2;


3. Compare Target:

If array[mid] == target, return the index.

If array[mid] < target, move the low pointer to mid + 1.

If array[mid] > target, move the high pointer to mid - 1.



4. Repeat: Continue the process until the target is found or the search space becomes empty.




---

📊 Time Complexity

Best Case: O(1) (Target is at the middle index on the first comparison).

Worst Case: O(log n) (Target is not present, and the array is divided until no elements remain).

Space Complexity: O(1) (Iterative approach) or O(log n) (Recursive approach due to call stack).



---

📝 Use Cases

Searching in large datasets, such as:

Phone directories

Sorted databases

Searching in gaming leaderboards

Word lookups in dictionaries
