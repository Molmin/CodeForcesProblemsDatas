## Description

<div><p>Your task is to calculate the number of arrays such that:</p><ul> <li> each array contains $n$ elements; </li><li> each element is an integer from $1$ to $m$; </li><li> for each array, there is <span class="tex-font-style-bf">exactly</span> one pair of equal elements; </li><li> for each array $a$, there exists an index $i$ such that the array is <span class="tex-font-style-bf">strictly ascending</span> before the $i$-th element and <span class="tex-font-style-bf">strictly descending</span> after it (formally, it means that $a_j &lt; a_{j + 1}$, if $j &lt; i$, and $a_j &gt; a_{j + 1}$, if $j \ge i$). </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le m \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print one integer — the number of arrays that meet all of the aforementioned conditions, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le m \le 2 \cdot 10^5$).</p>

## Output

<p>Print one integer — the number of arrays that meet all of the aforementioned conditions, taken modulo $998244353$.</p>





```input1
3 4
```




```input2
3 5
```




```input3
42 1337
```




```input4
100000 200000
```




```output1
6
```




```output2
10
```




```output3
806066790
```




```output4
707899035
```



## Note

<p>The arrays in the first example are:</p><ul> <li> $[1, 2, 1]$; </li><li> $[1, 3, 1]$; </li><li> $[1, 4, 1]$; </li><li> $[2, 3, 2]$; </li><li> $[2, 4, 2]$; </li><li> $[3, 4, 3]$. </li></ul>
