## Description

<div><p>Let's call an array $a$ of $m$ integers $a_1, a_2, \ldots, a_m$ <span class="tex-font-style-bf">Decinc</span> if $a$ can be made increasing by removing a decreasing subsequence (possibly empty) from it.</p><ul><li> For example, if $a = [3, 2, 4, 1, 5]$, we can remove the decreasing subsequence $[a_1, a_4]$ from $a$ and obtain $a = [2, 4, 5]$, which is increasing.</li></ul><p>You are given a permutation $p$ of numbers from $1$ to $n$. Find the number of pairs of integers $(l, r)$ with $1 \le l \le r \le n$ such that $p[l \ldots r]$ (the subarray of $p$ from $l$ to $r$) is a <span class="tex-font-style-bf">Decinc</span> array. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) &nbsp;— the size of $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— elements of the permutation.</p></div><div class="output-specification"><p>Output the number of pairs of integers $(l, r)$ such that $p[l \ldots r]$ (the subarray of $p$ from $l$ to $r$) is a <span class="tex-font-style-bf">Decinc</span> array. $(1 \le l \le r \le n)$</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) &nbsp;— the size of $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— elements of the permutation.</p>

## Output

<p>Output the number of pairs of integers $(l, r)$ such that $p[l \ldots r]$ (the subarray of $p$ from $l$ to $r$) is a <span class="tex-font-style-bf">Decinc</span> array. $(1 \le l \le r \le n)$</p>





```input1
3
2 3 1
```




```input2
6
4 5 2 6 1 3
```




```input3
10
7 10 1 8 3 9 2 4 6 5
```




```output1
6
```




```output2
19
```




```output3
39
```



## Note

<p>In the first sample, all subarrays are <span class="tex-font-style-bf">Decinc</span>.</p><p>In the second sample, all subarrays except $p[1 \ldots 6]$ and $p[2 \ldots 6]$ are <span class="tex-font-style-bf">Decinc</span>.</p>
