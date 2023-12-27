# Intuition
<!-- Describe your first thoughts on how to solve this problem. -->
- The code seems to implement a function to compress a character array by replacing consecutive repeating characters with the character and the count of repetitions.

---


# Approach
<!-- Describe your approach to solving the problem. -->
1. Initialize variables i and count.
2. Iterate through the vector chars starting from index j=1.
3. Check if chars[i] is not equal to chars[j]:
    - If count is greater than 1, append chars[i] and the string representation of count to the str.
    - If count is 1, append only chars[i] to the str.
    - Update i to j, set chars[i] to chars[j], and reset count to 1.
4. If the loop completes and count is greater than 1, append chars[i] and the string representation of count to the str.
5. Clear the original chars vector.
6. Populate chars vector with characters from the str.
7. Return the length of the compressed string (str).

---


# Complexity
- Time complexity:
<!-- Add your time complexity here, e.g. $$O(n)$$ -->
-  **O(n)** - *where n is the length of the input vector chars. The algorithm iterates through the vector once.*
- 

---


- Space complexity:
<!-- Add your space complexity here, e.g. $$O(n)$$ -->
- **O(1)** -* The space used is independent of the input size. The additional space used is for the variables, and it does not grow with the input size.*
- 

---
