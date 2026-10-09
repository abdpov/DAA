
№1) Problem
we have an array of integers, we need to sort it in ascending order, from smallest to largest

example: [5, 2, 3, 1]

result: [1, 2, 3, 5]
№2) Approach

i used Merge Sort, this algorithm divides the array into two parts, sorts each part, and then merges them back in the correct order
example: array [5, 2, 3, 1]
1. start: [5, 2, 3, 1]
2. step 1: divide the array into [5, 2] and [3, 1]
3. step 2: divide again into [5], [2], [3], [1]
4. step 3: merge [5] and [2] = [2, 5]
5. step 4: merge [3] and [1] = [1, 3]
6. step 5: merge [2, 5] and [1, 3] = [1, 2, 3, 5]

the main challenge is to merge the two parts in the correct order, because we need to compare their elements and always take the smaller one first

№3) Time Complexity

Time Complexity: O(n log n) because the array is divided into halves, so there are about log n levels, and merging all elements at each level takes O(n) time

Space Complexity: O(n) because we use an extra array to store elements while merging

№4) Reflection/Improvement

is there a more efficient approach? Merge Sort is already efficient in time because it takes O(n log n)

what would you need to change? we could use Heap Sort, which also takes O(n log n) time but uses O(1) extra space

what complexity could the improved solution achieve? Heap Sort can achieve O(n log n) time and O(1) extra space
