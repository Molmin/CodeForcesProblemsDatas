## Description

<div><p>At first, there was a legend related to the name of the problem, but now it's just a formal statement.</p><p>You are given $n$ points $a_1, a_2, \dots, a_n$ on the $OX$ axis. Now you are asked to find such an integer point $x$ on $OX$ axis that $f_k(x)$ is minimal possible.</p><p>The function $f_k(x)$ can be described in the following way: </p><ul> <li> form a list of distances $d_1, d_2, \dots, d_n$ where $d_i = |a_i - x|$ (distance between $a_i$ and $x$); </li><li> sort list $d$ in non-descending order; </li><li> take $d_{k + 1}$ as a result. </li></ul><p>If there are multiple optimal answers you can print any of them.</p></div><div class="input-specification"><p>The first line contains single integer $T$ ($ 1 \le T \le 2 \cdot 10^5$) — number of queries. Next $2 \cdot T$ lines contain descriptions of queries. All queries are independent. </p><p>The first line of each query contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k &lt; n$) — the number of points and constant $k$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_n \le 10^9$) — points in ascending order.</p><p>It's guaranteed that $\sum{n}$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $T$ integers — corresponding points $x$ which have minimal possible value of $f_k(x)$. If there are multiple answers you can print any of them.</p></div>

## Input

<p>The first line contains single integer $T$ ($ 1 \le T \le 2 \cdot 10^5$) — number of queries. Next $2 \cdot T$ lines contain descriptions of queries. All queries are independent. </p><p>The first line of each query contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k &lt; n$) — the number of points and constant $k$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_n \le 10^9$) — points in ascending order.</p><p>It's guaranteed that $\sum{n}$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $T$ integers — corresponding points $x$ which have minimal possible value of $f_k(x)$. If there are multiple answers you can print any of them.</p>





```input1
3
3 2
1 2 5
2 1
1 1000000000
1 0
4
```




```output1
3
500000000
4
```


