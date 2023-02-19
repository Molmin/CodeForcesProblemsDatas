## Description

<div><p>You are given an array $a$ consisting of $n$ integers. We denote the subarray $a[l..r]$ as the array $[a_l, a_{l + 1}, \dots, a_r]$ ($1 \le l \le r \le n$).</p><p>A subarray is considered <span class="tex-font-style-it">good</span> if every integer that occurs in this subarray occurs there <span class="tex-font-style-bf">exactly thrice</span>. For example, the array $[1, 2, 2, 2, 1, 1, 2, 2, 2]$ has three good subarrays:</p><ul> <li> $a[1..6] = [1, 2, 2, 2, 1, 1]$; </li><li> $a[2..4] = [2, 2, 2]$; </li><li> $a[7..9] = [2, 2, 2]$. </li></ul><p>Calculate the number of good subarrays of the given array $a$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le n$).</p></div><div class="output-specification"><p>Print one integer — the number of good subarrays of the array $a$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le n$).</p>

## Output

<p>Print one integer — the number of good subarrays of the array $a$.</p>





```input1
9
1 2 2 2 1 1 2 2 2
```




```input2
10
1 2 3 4 1 2 3 1 2 3
```




```input3
12
1 2 3 4 3 4 2 1 3 4 2 1
```




```output1
3
```




```output2
0
```




```output3
1
```


