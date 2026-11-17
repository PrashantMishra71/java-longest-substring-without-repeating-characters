# Longest Substring Without Repeating Characters

A Java solution to the Longest Substring Without Repeating Characters problem using the **Sliding Window** technique.

## Problem Statement

Given a string `s`, find the length of the longest substring without repeating characters.

## Example

**Input:**
```text
s = "abcabcbb"
```

**Output:**
```text
3
```

**Explanation:**

The longest substring without repeating characters is `"abc"`, with a length of 3.

## Approach: Sliding Window

- Use two pointers (`left` and `right`) to maintain a sliding window.
- Use a HashSet to store characters currently inside the window.
- Expand the window when a new character is encountered.
- If a duplicate character is found, shrink the window from the left.
- Maintain the maximum substring length.

## Complexity Analysis

- **Time Complexity:** O(n) — Each character is processed at most twice.
- **Space Complexity:** O(min(n, k)) — HashSet stores unique characters, where k is the character-set size.

## Language

Java

## Topic

- Sliding Window
- HashSet
- Two Pointers
- String Manipulation