## Description

<div><p>You are given a permutation $p$ consisting of $n$ integers $1, 2, \dots, n$ (a permutation is an array where each element from $1$ to $n$ occurs exactly once).</p><p>Let's call an array $a$ <span class="tex-font-style-it">bipartite</span> if the following undirected graph is bipartite:</p><ul> <li> the graph consists of $n$ vertices; </li><li> two vertices $i$ and $j$ are connected by an edge if $i &lt; j$ and $a_i &gt; a_j$. </li></ul><p>Your task is to find a <span class="tex-font-style-it">bipartite</span> array of integers $a$ of size $n$, such that $a_i = p_i$ or $a_i = -p_i$, or report that no such array exists. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$.</p><p>The sum of $n$ over all test cases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print the answer in the following format. If such an array $a$ does not exist, print "<span class="tex-font-style-tt">NO</span>" in a single line. Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and $n$ integers&nbsp;— array $a$ in the second line.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$.</p><p>The sum of $n$ over all test cases doesn't exceed $10^6$.</p>

## Output

<p>For each test case, print the answer in the following format. If such an array $a$ does not exist, print "<span class="tex-font-style-tt">NO</span>" in a single line. Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and $n$ integers&nbsp;— array $a$ in the second line.</p>





```input1
4
3
1 2 3
6
1 3 2 6 5 4
4
4 1 3 2
8
3 2 1 6 7 8 5 4
```




```output1
YES
1 2 3
NO
YES
-4 -1 -3 -2
YES
-3 -2 1 6 7 -8 -5 -4
```


