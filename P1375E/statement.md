## Description

<div><p>Madeline has an array $a$ of $n$ integers. A pair $(u, v)$ of integers forms an inversion in $a$ if:</p><ul> <li> $1 \le u &lt; v \le n$. </li><li> $a_u &gt; a_v$. </li></ul><p>Madeline recently found a magical paper, which allows her to write two indices $u$ and $v$ and swap the values $a_u$ and $a_v$. Being bored, she decided to write a list of pairs $(u_i, v_i)$ with the following conditions:</p><ul> <li> all the pairs in the list are distinct and form an inversion in $a$. </li><li> all the pairs that form an inversion in $a$ are in the list. </li><li> Starting from the given array, if you swap the values at indices $u_1$ and $v_1$, then the values at indices $u_2$ and $v_2$ and so on, then after all pairs are processed, the array $a$ will be sorted in <span class="tex-font-style-bf">non-decreasing order</span>. </li></ul><p>Construct such a list or determine that no such list exists. If there are multiple possible answers, you may find any of them.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 1000$) — the length of the array.</p><p>Next line contains $n$ integers $a_1,a_2,...,a_n$ $(1 \le a_i \le 10^9)$ &nbsp;— elements of the array.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if no such list exists. Otherwise in the first line you should print a single integer $m$ ($0 \le m \le \dfrac{n(n-1)}{2}$) — number of pairs in the list.</p><p>The $i$-th of the following $m$ lines should contain two integers $u_i, v_i$ ($1 \le u_i &lt; v_i\le n$).</p><p>If there are multiple possible answers, you may find any of them.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 1000$) — the length of the array.</p><p>Next line contains $n$ integers $a_1,a_2,...,a_n$ $(1 \le a_i \le 10^9)$ &nbsp;— elements of the array.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if no such list exists. Otherwise in the first line you should print a single integer $m$ ($0 \le m \le \dfrac{n(n-1)}{2}$) — number of pairs in the list.</p><p>The $i$-th of the following $m$ lines should contain two integers $u_i, v_i$ ($1 \le u_i &lt; v_i\le n$).</p><p>If there are multiple possible answers, you may find any of them.</p>





```input1
3
3 1 2
```




```input2
4
1 8 1 6
```




```input3
5
1 1 1 2 2
```




```output1
2
1 3
1 2
```




```output2
2
2 4
2 3
```




```output3
0
```



## Note

<p>In the first sample test case the array will change in this order $[3,1,2] \rightarrow [2,1,3] \rightarrow [1,2,3]$.</p><p>In the second sample test case it will be $[1,8,1,6] \rightarrow [1,6,1,8] \rightarrow [1,1,6,8]$.</p><p>In the third sample test case the array is already sorted.</p>
