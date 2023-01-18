## Description

<div><p>You are given an array $a$ consisting of $n$ integers. Beauty of array is the maximum sum of some <span class="tex-font-style-bf">consecutive subarray</span> of this array (this subarray may be empty). For example, the beauty of the array <span class="tex-font-style-tt">[10, -5, 10, -4, 1]</span> is <span class="tex-font-style-tt">15</span>, and the beauty of the array <span class="tex-font-style-tt">[-3, -5, -1]</span> is <span class="tex-font-style-tt">0</span>.</p><p>You may choose <span class="tex-font-style-bf">at most one consecutive subarray</span> of $a$ and multiply all values contained in this subarray by $x$. You want to maximize the beauty of array after applying at most one such operation.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $x$ ($1 \le n \le 3 \cdot 10^5, -100 \le x \le 100$) — the length of array $a$ and the integer $x$ respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — the array $a$.</p></div><div class="output-specification"><p>Print one integer — the maximum possible beauty of array $a$ after multiplying all values belonging to some consecutive subarray $x$.</p></div>

## Input

<p>The first line contains two integers $n$ and $x$ ($1 \le n \le 3 \cdot 10^5, -100 \le x \le 100$) — the length of array $a$ and the integer $x$ respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — the array $a$.</p>

## Output

<p>Print one integer — the maximum possible beauty of array $a$ after multiplying all values belonging to some consecutive subarray $x$.</p>





```input1
5 -2
-3 8 -2 1 -6
```




```input2
12 -3
1 3 3 7 1 3 3 7 1 3 3 7
```




```input3
5 10
-1 -2 -3 -4 -5
```




```output1
22
```




```output2
42
```




```output3
0
```



## Note

<p>In the first test case we need to multiply the subarray <span class="tex-font-style-tt">[-2, 1, -6]</span>, and the array becomes <span class="tex-font-style-tt">[-3, 8, 4, -2, 12]</span> with beauty <span class="tex-font-style-tt">22</span> (<span class="tex-font-style-tt">[-3, <span class="tex-font-style-bf">8, 4, -2, 12</span>]</span>).</p><p>In the second test case we don't need to multiply any subarray at all.</p><p>In the third test case no matter which subarray we multiply, the beauty of array will be equal to <span class="tex-font-style-tt">0</span>.</p>
