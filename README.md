<h1>Group 1 (Beginner Div)</h1>

<h2>A</h2>
Amy is given two positive integers, n and m. She defines 2 values, num1 and num2, as follows:</br>
- num1: The sum of all integers in the range from 1 to n (inclusive) that are not divisible by m.</br>
- num2: The sum of all integers in the range from 1 to n (inclusive) that are divisible by m.

Now, provide the result of subtracting num2 from num1.

**Example 1:**

**Input:** n = 10, m = 3`<br>`
**Output:** 19`<br>`
**Explanation:**
In the given example:

- Integers in the range [1, 10] that are not divisible by 3 are [1,2,4,5,7,8,10], num1 is the sum of those integers = 37.
- Integers in the range [1, 10] that are divisible by 3 are [3,6,9], num2 is the sum of those integers = 18.
  We return 37 - 18 = 19 as the answer.

**Example 2:**

**Input:** n = 5, m = 6`<br>`
**Output:** 15`<br>`
**Explanation:**
In the given example:

- Integers in the range [1, 5] that are not divisible by 6 are [1,2,3,4,5], num1 is the sum of those integers = 15.
- Integers in the range [1, 5] that are divisible by 6 are [], num2 is the sum of those integers = 0.
  We return 15 - 0 = 15 as the answer.

**Example 3:**

**Input:** n = 5, m = 1`<br>`
**Output:** -15`<br>`
**Explanation:**
In the given example:

- Integers in the range [1, 5] that are not divisible by 1 are [], num1 is the sum of those integers = 0.
- Integers in the range [1, 5] that are divisible by 1 are [1,2,3,4,5], num2 is the sum of those integers = 15.
  We return 0 - 15 = -15 as the answer.

**Constraints:**

- 1 <= n, m <= 1000

<h2>B</h2>
You are given a positive integer array `nums`.

The element sum is the sum of all the elements in `nums`.
The digit sum is the sum of all the digits (not necessarily distinct) that appear in `nums`.
Return the absolute difference between the element sum and digit sum of `nums`.

Note that the absolute difference between two integers x and y is defined as |x - y|.

**Example 1:**

**Input:** `nums = [1,15,6,3]<br>`
**Output:** `9<br>`
**Explanation:**
The element sum of `nums` is 1 + 15 + 6 + 3 = 25.
The digit sum of `nums` is 1 + 1 + 5 + 6 + 3 = 16.
The absolute difference between the element sum and digit sum is |25 - 16| = 9.

**Example 2:**

**Input:** `nums = [1,2,3,4]<br>`
**Output:** `0<br>`
**Explanation:**
The element sum of `nums` is 1 + 2 + 3 + 4 = 10.
The digit sum of `nums` is 1 + 2 + 3 + 4 = 10.
The absolute difference between the element sum and digit sum is |10 - 10| = 0.

**Constraints:**

- `1 <= nums.length <= 2000`
- `1 <= nums[i] <= 2000`

<h1>Group 2 (Intermediate Div)</h1>
<h2>A</h2>
Given a 2D integer array `matrix`, return the transpose of the matrix.

The transpose of a matrix is the matrix flipped over its main diagonal, switching the matrix's row and column indices.

![](https://cdn.discordapp.com/attachments/777732038324256779/1164281049552015420/image.png?ex=6542a439&is=65302f39&hm=ede6732aa5730ec719b7e7ecb828a70977224ba57b3225ae0de9f0227853d17a&)
**Example 1:**

**Input:** `matrix = [[1,2,3],[4,5,6],[7,8,9]]`

**Output:** `[[1,4,7],[2,5,8],[3,6,9]]`

**Example 2:**

**Input:** `matrix = [[1,2,3],[4,5,6]]`

**Output:** `[[1,4],[2,5],[3,6]]`

**Constraints:**

- `m == matrix.length`
- `n == matrix[i].length`
- `1 <= m, n <= 1000`
- `1 <= m * n <= 105`
- `-109 <= matrix[i][j] <= 109`

<h2>B</h2>
An array `nums` of length `n` is beautiful if:

- `nums` is a permutation of the integers in the range `[1, n]`.
- For every `0 <= i < j < n`, there is no index `k` with `i < k < j` where `2 * nums[k] == nums[i] + nums[j]`.

Given the integer `n`, return any beautiful array `nums` of length `n`. There will be at least one valid answer for the given `n`.

**Example 1:**

**Input:** `n = 4`
**Output:** `[2,1,4,3]`

**Example 2:**

**Input:** `n = 5`
**Output:** `[3,1,2,5,4]`

**Constraints:**

- `1 <= n <= 1000`
