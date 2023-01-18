## Description

<div><p>You are given $n$ pairs of integers $(a_1, b_1), (a_2, b_2), \ldots, (a_n, b_n)$. All of the integers in the pairs are distinct and are in the range from $1$ to $2 \cdot n$ inclusive.</p><p>Let's call a sequence of integers $x_1, x_2, \ldots, x_{2k}$ <span class="tex-font-style-it">good</span> if either </p><ul> <li> $x_1 &lt; x_2 &gt; x_3 &lt; \ldots &lt; x_{2k-2} &gt; x_{2k-1} &lt; x_{2k}$, or </li><li> $x_1 &gt; x_2 &lt; x_3 &gt; \ldots &gt; x_{2k-2} &lt; x_{2k-1} &gt; x_{2k}$. </li></ul><p>You need to choose a subset of distinct indices $i_1, i_2, \ldots, i_t$ and <span class="tex-font-style-bf">their order</span> in a way that if you write down all numbers from the pairs in a single sequence (the sequence would be $a_{i_1}, b_{i_1}, a_{i_2}, b_{i_2}, \ldots, a_{i_t}, b_{i_t}$), this sequence is good.</p><p>What is the largest subset of indices you can choose? You also need to construct the corresponding index sequence $i_1, i_2, \ldots, i_t$.</p></div><div class="input-specification"><p>The first line contains single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$)&nbsp;— the number of pairs.</p><p>Each of the next $n$ lines contain two numbers&nbsp;— $a_i$ and $b_i$ ($1 \le a_i, b_i \le 2 \cdot n$)&nbsp;— the elements of the pairs.</p><p>It is guaranteed that all integers in the pairs are distinct, that is, every integer from $1$ to $2 \cdot n$ is mentioned exactly once.</p></div><div class="output-specification"><p>In the first line print a single integer $t$&nbsp;— the number of pairs in the answer.</p><p>Then print $t$ distinct integers $i_1, i_2, \ldots, i_t$&nbsp;— the indexes of pairs in the corresponding order.</p></div>

## Input

<p>The first line contains single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$)&nbsp;— the number of pairs.</p><p>Each of the next $n$ lines contain two numbers&nbsp;— $a_i$ and $b_i$ ($1 \le a_i, b_i \le 2 \cdot n$)&nbsp;— the elements of the pairs.</p><p>It is guaranteed that all integers in the pairs are distinct, that is, every integer from $1$ to $2 \cdot n$ is mentioned exactly once.</p>

## Output

<p>In the first line print a single integer $t$&nbsp;— the number of pairs in the answer.</p><p>Then print $t$ distinct integers $i_1, i_2, \ldots, i_t$&nbsp;— the indexes of pairs in the corresponding order.</p>





```input1
5
1 7
6 4
2 10
9 8
3 5
```




```input2
3
5 4
3 2
6 1
```




```output1
3
1 5 3
```




```output2
3
3 2 1
```



## Note

<p>The final sequence in the first example is $1 &lt; 7 &gt; 3 &lt; 5 &gt; 2 &lt; 10$.</p><p>The final sequence in the second example is $6 &gt; 1 &lt; 3 &gt; 2 &lt; 5 &gt; 4$.</p>
