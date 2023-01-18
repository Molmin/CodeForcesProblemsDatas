## Description

<div><p>Recently, on the course of algorithms and data structures, Valeriy learned how to use a deque. He built a deque filled with $n$ elements. The $i$-th element is $a_i$ ($i$ = $1, 2, \ldots, n$). He gradually takes the first two leftmost elements from the deque (let's call them $A$ and $B$, respectively), and then does the following: if $A &gt; B$, he writes $A$ to the beginning and writes $B$ to the end of the deque, otherwise, he writes to the beginning $B$, and $A$ writes to the end of the deque. We call this sequence of actions an operation.</p><p>For example, if deque was $[2, 3, 4, 5, 1]$, on the operation he will write $B=3$ to the beginning and $A=2$ to the end, so he will get $[3, 4, 5, 1, 2]$.</p><p>The teacher of the course, seeing Valeriy, who was passionate about his work, approached him and gave him $q$ queries. Each query consists of the singular number $m_j$ $(j = 1, 2, \ldots, q)$. It is required for each query to answer which two elements he will pull out on the $m_j$-th operation.</p><p>Note that <span class="tex-font-style-bf">the queries are independent</span> and for each query the numbers $A$ and $B$ should be <span class="tex-font-style-bf">printed in the order in which they will be pulled out of the deque</span>.</p><p><span class="tex-font-style-it">Deque</span> is a data structure representing a list of elements where insertion of new elements or deletion of existing elements can be made from both sides.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \leq n \leq 10^5$, $0 \leq q \leq 3 \cdot 10^5$)&nbsp;— the number of elements in the deque and the number of queries. The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$, where $a_i$ $(0 \leq a_i \leq 10^9)$&nbsp;— the deque element in $i$-th position. The next $q$ lines contain one number each, meaning $m_j$ ($1 \leq m_j \leq 10^{18}$).</p></div><div class="output-specification"><p>For each teacher's query, output two numbers $A$ and $B$&nbsp;— the numbers that Valeriy pulls out of the deque for the $m_j$-th operation.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \leq n \leq 10^5$, $0 \leq q \leq 3 \cdot 10^5$)&nbsp;— the number of elements in the deque and the number of queries. The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$, where $a_i$ $(0 \leq a_i \leq 10^9)$&nbsp;— the deque element in $i$-th position. The next $q$ lines contain one number each, meaning $m_j$ ($1 \leq m_j \leq 10^{18}$).</p>

## Output

<p>For each teacher's query, output two numbers $A$ and $B$&nbsp;— the numbers that Valeriy pulls out of the deque for the $m_j$-th operation.</p>





```input1
5 3
1 2 3 4 5
1
2
10
```




```input2
2 0
0 0
```




```output1
1 2
2 3
5 2
```




```output2

```



## Note

<ol> Consider all 10 steps for the first test in detail:<li> $[1, 2, 3, 4, 5]$&nbsp;— on the first operation, $A$ and $B$ are $1$ and $2$, respectively.<p>So, $2$ we write to the beginning of the deque, and $1$&nbsp;— to the end.</p><p>We get the following status of the deque: $[2, 3, 4, 5, 1]$.</p></li><li> $[2, 3, 4, 5, 1] \Rightarrow A = 2, B = 3$.</li><li> $[3, 4, 5, 1, 2]$</li><li> $[4, 5, 1, 2, 3]$</li><li> $[5, 1, 2, 3, 4]$</li><li> $[5, 2, 3, 4, 1]$</li><li> $[5, 3, 4, 1, 2]$</li><li> $[5, 4, 1, 2, 3]$</li><li> $[5, 1, 2, 3, 4]$</li><li> $[5, 2, 3, 4, 1] \Rightarrow A = 5, B = 2$. </li></ol>
