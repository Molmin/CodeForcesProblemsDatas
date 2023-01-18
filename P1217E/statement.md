## Description

<div><p>Let's define a <span class="tex-font-style-it">balanced</span> multiset the following way. Write down the sum of all elements of the multiset in its decimal representation. For each position of that number check if the multiset includes at least one element such that the digit of the element and the digit of the sum at that position are the same. If that holds for every position, then the multiset is <span class="tex-font-style-it">balanced</span>. Otherwise it's <span class="tex-font-style-it">unbalanced</span>.</p><p>For example, multiset $\{20, 300, 10001\}$ is <span class="tex-font-style-it">balanced</span> and multiset $\{20, 310, 10001\}$ is <span class="tex-font-style-it">unbalanced</span>: </p><center> <img class="tex-graphics" src="file://hKpEBKu2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The red digits mark the elements and the positions for which these elements have the same digit as the sum. The sum of the first multiset is $10321$, every position has the digit required. The sum of the second multiset is $10331$ and the second-to-last digit doesn't appear in any number, thus making the multiset <span class="tex-font-style-it">unbalanced</span>.</p><p>You are given an array $a_1, a_2, \dots, a_n$, consisting of $n$ integers.</p><p>You are asked to perform some queries on it. The queries can be of two types:</p><ul> <li> $1~i~x$ — replace $a_i$ with the value $x$; </li><li> $2~l~r$ — find the <span class="tex-font-style-bf"><span class="tex-font-style-it">unbalanced</span></span> subset of the multiset of the numbers $a_l, a_{l + 1}, \dots, a_r$ with the minimum sum, or report that no <span class="tex-font-style-it">unbalanced</span> subset exists. </li></ul><p>Note that the empty multiset is <span class="tex-font-style-it">balanced</span>.</p><p>For each query of the second type print the lowest sum of the <span class="tex-font-style-it">unbalanced</span> subset. Print <span class="tex-font-style-tt">-1</span> if no <span class="tex-font-style-it">unbalanced</span> subset exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of elements in the array and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i &lt; 10^9$).</p><p>Each of the following $m$ lines contains a query of one of two types:</p><ul> <li> $1~i~x$ ($1 \le i \le n$, $1 \le x &lt; 10^9$) — replace $a_i$ with the value $x$; </li><li> $2~l~r$ ($1 \le l \le r \le n$) — find the <span class="tex-font-style-bf"><span class="tex-font-style-it">unbalanced</span></span> subset of the multiset of the numbers $a_l, a_{l + 1}, \dots, a_r$ with the lowest sum, or report that no <span class="tex-font-style-it">unbalanced</span> subset exists. </li></ul><p>It is guaranteed that there is at least one query of the second type.</p></div><div class="output-specification"><p>For each query of the second type print the lowest sum of the <span class="tex-font-style-it">unbalanced</span> subset. Print <span class="tex-font-style-tt">-1</span> if no <span class="tex-font-style-it">unbalanced</span> subset exists.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of elements in the array and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i &lt; 10^9$).</p><p>Each of the following $m$ lines contains a query of one of two types:</p><ul> <li> $1~i~x$ ($1 \le i \le n$, $1 \le x &lt; 10^9$) — replace $a_i$ with the value $x$; </li><li> $2~l~r$ ($1 \le l \le r \le n$) — find the <span class="tex-font-style-bf"><span class="tex-font-style-it">unbalanced</span></span> subset of the multiset of the numbers $a_l, a_{l + 1}, \dots, a_r$ with the lowest sum, or report that no <span class="tex-font-style-it">unbalanced</span> subset exists. </li></ul><p>It is guaranteed that there is at least one query of the second type.</p>

## Output

<p>For each query of the second type print the lowest sum of the <span class="tex-font-style-it">unbalanced</span> subset. Print <span class="tex-font-style-tt">-1</span> if no <span class="tex-font-style-it">unbalanced</span> subset exists.</p>





```input1
4 5
300 10001 20 20
2 1 3
1 1 310
2 1 3
2 3 3
2 3 4
```




```output1
-1
330
-1
40
```



## Note

<p>All the subsets of multiset $\{20, 300, 10001\}$ are <span class="tex-font-style-it">balanced</span>, thus the answer is <span class="tex-font-style-tt">-1</span>.</p><p>The possible <span class="tex-font-style-it">unbalanced</span> subsets in the third query are $\{20, 310\}$ and $\{20, 310, 10001\}$. The lowest sum one is $\{20, 310\}$. Note that you are asked to choose a subset, not a subsegment, thus the chosen elements might not be adjancent in the array.</p><p>The fourth query includes only the empty subset and subset $\{20\}$. Both of them are <span class="tex-font-style-it">balanced</span>.</p><p>The last query includes the empty subset and the subsets $\{20\}$, $\{20\}$ and $\{20, 20\}$. Only $\{20, 20\}$ is <span class="tex-font-style-it">unbalanced</span>, its sum is $40$. Note that you are asked to choose a multiset, thus it might include equal elements.</p>
