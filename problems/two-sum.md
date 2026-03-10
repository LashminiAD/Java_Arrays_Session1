# Two Sum (#1 LeetCode)

## Problem

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

You may assume that each input would have **exactly one solution**, and you may not use the same element twice.

---

## Example

**Input**

nums = [2,7,11,15]  
target = 9

**Output**

[0,1]

---

## Explanation

nums[0] = 2  
nums[1] = 7  
2 + 7 = 9  

So we return indices **[0, 1]**.

---

## Brute Force Idea

Step 1: Pick the first element  
Step 2: Compare it with every other element  
Step 3: Check if their sum equals the target  
Step 4: If yes → return the indices  

---

## Optimized Idea (HashMap)

Use a `HashMap` to store:

- **key** = number
- **value** = index

For each number `nums[i]`, compute:

complement = target - nums[i]

If complement exists in the map → we found the pair.

---

## Time Complexity

- Brute Force: **O(n²)**
- Optimized (HashMap): **O(n)**

---

## Space Complexity

- Brute Force: **O(1)**
- Optimized (HashMap): **O(n)**
