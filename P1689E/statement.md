## Description

<div><p><span class="tex-font-style-it">Bit Lightyear, to the ANDfinity and beyond!</span></p><p>After graduating from computer sciences, Vlad has been awarded an array $a_1,a_2,\ldots,a_n$ of $n$ non-negative integers. As it is natural, he wanted to construct a graph consisting of $n$ vertices, numbered $1, 2,\ldots, n$. He decided to add an edge between $i$ and $j$ if and only if $a_i \&amp; a_j &gt; 0$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Vlad also wants the graph to be connected, which might not be the case initially. In order to satisfy that, he can do the following two types of operations on the array:</p><ol> <li> Choose some element $a_i$ and increment it by $1$. </li><li> Choose some element $a_i$ and decrement it by $1$ (possible only if $a_i &gt; 0$). </li></ol><p>It can be proven that there exists a finite sequence of operations such that the graph will be connected. So, can you please help Vlad find the minimum possible number of operations to do that and also provide the way how to do that?</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains an integer $n$ ($2\leq n \leq 2000$). </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i &lt; 2^{30}$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, print a single integer $m$ in the first line&nbsp;— the minimum number of operations. In the second line print the array after a valid sequence of operations that have been done such that the graph from the task becomes connected. </p><p>If there are multiple solutions, output any.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains an integer $n$ ($2\leq n \leq 2000$). </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i &lt; 2^{30}$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, print a single integer $m$ in the first line&nbsp;— the minimum number of operations. In the second line print the array after a valid sequence of operations that have been done such that the graph from the task becomes connected. </p><p>If there are multiple solutions, output any.</p>





```input1
4
5
1 2 3 4 5
2
0 2
2
3 12
4
3 0 0 0
```




```output1
0
1 2 3 4 5
2
2 2
1
3 11
3
3 1 1 1
```



## Note

<p>In the first test case, the graph is already connected.</p><p>In the second test case, we can increment $0$ twice and end up with the array $[2,2]$. Since $2 \&amp; 2 = 2 &gt; 0$, the graph is connected. It can be shown that one operation is not enough.</p><p>In the third test case, we can decrement $12$ once and we end up with an array $[3,11]$. $3 \&amp; 11 = 3 &gt; 0$ hence the graph is connected. One operation has to be done since the graph is not connected at the beginning.</p>
