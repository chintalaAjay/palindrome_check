# Palindrome String - GFG Solution

This repository contains my Java solution for the **Palindrome String** problem from GeeksforGeeks.

## Problem Link
https://www.geeksforgeeks.org/problems/palindrome-string0817/1

---

## Problem Statement

Given a string `s`, check whether the string is a palindrome or not.

A palindrome is a string that reads the same forward and backward.

---

## My Approach

In this solution:

- Created a temporary character array
- Copied all characters from the string into the array
- Compared characters from the beginning and end
- Returned `false` if any mismatch was found
- Returned `true` if all characters matched

---

## Java Solution

```java
class Solution {
    boolean isPalindrome(String s) {

        boolean ispal = true;

        char arr[] = new char[s.length()];

        int k = s.length() - 1;

        for(int i = 0; i <= k; i++) {
            arr[i] = s.charAt(i);
        }

        for(int i = 0; i <= k; i++) {

            if(arr[i] != arr[k]) {
                return false;
            }

            k--;
        }

        return true;
    }
}
Example

Input:

madam

Output:

true
Concepts Used
Strings
Character Arrays
Traversing Arrays
Palindrome Checking
Time Complexity
O(n)
Space Complexity
O(n)

Extra space is used for the temporary character array.

Learning Outcome

Through this problem, I practiced:

String traversal
Character array handling in Java
Comparing elements using two directions
Basic palindrome logic

⭐ Practicing DSA consistently and uploading solutions to GitHub.
