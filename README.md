# HackerRank 3rd Semester Algorithm Portfolio

## Student Information

- **Name:** G Bhavana Reddy
- **USN:** R25EF082
- **Semester:** 3rd Semester
- **Programming Language:** Java

## Profiles

- **HackerRank:** https://www.hackerrank.com/profile/ugcet2501956
- **GitHub Repository:** https://github.com/BhavanaReddy1001/HackerRank-3rdSem-Algorithm-Portfolio

---

## Problem Portfolio

| No. | Problem | Approach | Time Complexity | Space Complexity |
|-----|---------|----------|-----------------|------------------|
| 1 | Mini-Max Sum | Find total sum, minimum and maximum values in one traversal | O(N) | O(1) |
| 2 | Birthday Cake Candles | Find the maximum candle height and count its occurrences | O(N) | O(1) |
| 3 | Insertion Sort – Part 1 | Shift larger elements and insert the selected value into its correct position | O(N) for the shifting operation | O(1) |
| 4 | Binary Search | Repeatedly divide the sorted search range into two halves | O(log N) | O(1) |
| 5 | Mark and Toys | Sort prices and greedily purchase the cheapest toys within the budget | O(N log N) | O(N) |

---

## 1. Mini-Max Sum

### Description

Given five positive integers, calculate the minimum and maximum values that can be obtained by summing exactly four of the five integers.

### Approach

The array is traversed once while keeping track of:

- Total sum
- Minimum value
- Maximum value

The minimum sum is obtained by excluding the maximum value, while the maximum sum is obtained by excluding the minimum value.

### Complexity

- **Time:** O(N)
- **Space:** O(1)

### HackerRank Challenge

https://www.hackerrank.com/challenges/mini-max-sum/problem

### Solution

`01-Mini-Max-Sum/solution.java`

---

## 2. Birthday Cake Candles

### Description

Given the heights of candles, determine how many candles have the maximum height.

### Approach

Traverse the list once.

Whenever a new maximum height is found, update the maximum and reset the count to 1. If the current height equals the maximum, increment the count.

### Complexity

- **Time:** O(N)
- **Space:** O(1)

### HackerRank Challenge

https://www.hackerrank.com/challenges/birthday-cake-candles/problem

### Solution

`02-Birthday-Cake-Candles/solution.java`

---

## 3. Insertion Sort – Part 1

### Description

Insert the last element of the array into its correct position in the already sorted portion of the array.

### Approach

Store the last element as the value to be inserted. Compare it with elements from right to left. Larger elements are shifted one position to the right until the correct position is found.

### Complexity

- **Time:** O(N) for the insertion/shifting operation
- **Space:** O(1)

### HackerRank Challenge

https://www.hackerrank.com/challenges/insertionsort1/problem

### Solution

`03-Insertion-Sort-Part-1/solution.java`

---

## 4. Binary Search

### Description

Binary Search is used to find a target element in a sorted array.

### Approach

Two pointers, `left` and `right`, represent the current search range. The middle element is calculated and compared with the target.

- If the middle element equals the target, its index is returned.
- If the middle element is smaller, search continues in the right half.
- If the middle element is larger, search continues in the left half.

The process continues until the element is found or the search range becomes empty.

### Complexity

- **Time:** O(log N)
- **Space:** O(1)

### Implementation

This problem was implemented independently in Java using a sorted integer array, as permitted by the activity instructions.

### Solution

`04-Binary-Search/BinarySearch.java`

---

## 5. Mark and Toys

### Description

Given the prices of toys and a fixed budget, determine the maximum number of toys that can be purchased.

### Approach

First, sort the toy prices in ascending order. Then purchase the cheapest toys one by one until the budget is insufficient.

### Complexity

- **Time:** O(N log N)
- **Space:** O(N) worst case due to the sorting implementation

### HackerRank Challenge

https://www.hackerrank.com/challenges/mark-and-toys/problem

### Solution

`05-Mark-and-Toys/solution.java`

---

## Repository Structure

```text
HackerRank-3rdSem-Algorithm-Portfolio/
│
├── 01-Mini-Max-Sum/
│   └── solution.java
│
├── 02-Birthday-Cake-Candles/
│   └── solution.java
│
├── 03-Insertion-Sort-Part-1/
│   └── solution.java
│
├── 04-Binary-Search/
│   └── BinarySearch.java
│
├── 05-Mark-and-Toys/
│   └── solution.java
│
└── README.md
