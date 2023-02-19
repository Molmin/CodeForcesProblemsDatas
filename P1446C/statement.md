## Description

<div><p>For a given sequence of <span class="tex-font-style-bf">distinct</span> non-negative integers $(b_1, b_2, \dots, b_k)$ we determine if it is <span class="tex-font-style-bf">good</span> in the following way:</p><ul> <li> Consider a graph on $k$ nodes, with numbers from $b_1$ to $b_k$ written on them.</li><li> For every $i$ from $1$ to $k$: find such $j$ ($1 \le j \le k$, $j\neq i$), for which $(b_i \oplus b_j)$ <span class="tex-font-style-bf">is the smallest</span> among all such $j$, where $\oplus$ denotes the operation of bitwise XOR (<a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">https://en.wikipedia.org/wiki/Bitwise_operation#XOR</a>). Next, draw an <span class="tex-font-style-bf">undirected</span> edge between vertices with numbers $b_i$ and $b_j$ in this graph.</li><li> We say that the sequence is <span class="tex-font-style-bf">good</span> if and only if the resulting graph forms a <span class="tex-font-style-bf">tree</span> (is connected and doesn't have any simple cycles). </li></ul><p>It is possible that for some numbers $b_i$ and $b_j$, you will try to add the edge between them twice. Nevertheless, you will add this edge only once.</p><p>You can find an example below (the picture corresponding to the first test case). </p><p>Sequence $(0, 1, 5, 2, 6)$ <span class="tex-font-style-bf">is not</span> good as we <span class="tex-font-style-bf">cannot</span> reach $1$ from $5$.</p><p>However, sequence $(0, 1, 5, 2)$ <span class="tex-font-style-bf">is</span> good. </p><center> <img class="tex-graphics" src="file://uLRigUxd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a sequence $(a_1, a_2, \dots, a_n)$ of <span class="tex-font-style-bf">distinct</span> non-negative integers. You would like to remove some of the elements (possibly none) to make the <span class="tex-font-style-bf">remaining</span> sequence good. What is the minimum possible number of removals required to achieve this goal?</p><p>It can be shown that for any sequence, we can remove some number of elements, leaving at least $2$, so that the remaining sequence is good.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 200,000$)&nbsp;— length of the sequence.</p><p>The second line contains $n$ <span class="tex-font-style-bf">distinct</span> non-negative integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the elements of the sequence.</p></div><div class="output-specification"><p>You should output exactly one integer&nbsp;— the minimum possible number of elements to remove in order to make the remaining sequence good.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 200,000$)&nbsp;— length of the sequence.</p><p>The second line contains $n$ <span class="tex-font-style-bf">distinct</span> non-negative integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the elements of the sequence.</p>

## Output

<p>You should output exactly one integer&nbsp;— the minimum possible number of elements to remove in order to make the remaining sequence good.</p>





```input1
5
0 1 5 2 6
```




```input2
7
6 9 8 7 3 5 2
```




```output1
1
```




```output2
2
```



## Note

<p>Note that numbers which you remove <span class="tex-font-style-bf">don't</span> impact the procedure of telling whether the resulting sequence is good.</p><p>It is possible that for some numbers $b_i$ and $b_j$, you will try to add the edge between them twice. Nevertheless, you will add this edge only once.</p>
