## Description

<div><p>You have an array $a$ of length $n$. You can <span class="tex-font-style-bf">exactly</span> once select an integer $len$ between $1$ and $n - 1$ inclusively, and then sort in non-decreasing order the prefix of the array of length $len$ and the suffix of the array of length $n - len$ independently.</p><p>For example, if the array is $a = [3, 1, 4, 5, 2]$, and you choose $len = 2$, then after that the array will be equal to $[1, 3, 2, 4, 5]$.</p><p>Could it be that after performing this operation, the array will <span class="tex-font-style-bf">not</span> be sorted in non-decreasing order?</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^4$)&nbsp;— the length of the array.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — the array elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case of input data, output "<span class="tex-font-style-tt">YES</span>" (without quotes), if the array may be <span class="tex-font-style-bf">not</span> sorted in non-decreasing order, output "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can output each letter in any case (uppercase or lowercase).</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^4$)&nbsp;— the length of the array.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — the array elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For each test case of input data, output "<span class="tex-font-style-tt">YES</span>" (without quotes), if the array may be <span class="tex-font-style-bf">not</span> sorted in non-decreasing order, output "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can output each letter in any case (uppercase or lowercase).</p>





```input1
3
3
2 2 1
4
3 1 2 1
5
1 2 2 4 4
```




```output1
YES
YES
NO
```



## Note

<p>In the first test case, it's possible to select $len = 1$, then after operation, the array will not be sorted in non-decreasing order and will be equal to $[2, 1, 2]$.</p><p>In the second test case, it's possible to select $len = 3$, then after operation, the array will not be sorted in non-decreasing order and will be equal to $[1, 2, 3, 1]$.</p><p>In the third test case, the array will be sorted in non-decreasing order for every possible $len$.</p>
