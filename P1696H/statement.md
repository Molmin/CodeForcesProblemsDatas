## Description

<div><p>You are given a positive integer $k$. For a multiset of integers $S$, define $f(S)$ as the following.</p><ul> <li> If the number of elements in $S$ is less than $k$, $f(S)=0$. </li><li> Otherwise, define $f(S)$ as the maximum product you can get by choosing exactly $k$ integers from $S$. </li></ul><p>More formally, let $|S|$ denote the number of elements in $S$. Then,</p><ul> <li> If $|S|&lt;k$, $f(S)=0$. </li><li> Otherwise, $f(S)=\max\limits_{T\subseteq S,|T|=k}\left(\prod\limits_{i\in T}i\right)$. </li></ul><p>You are given a multiset of integers, $A$. Compute $\sum\limits_{B\subseteq A} f(B)$ modulo $10^9+7$.</p><p>Note that in this problem, <span class="tex-font-style-bf">we distinguish the elements by indices instead of values</span>. That is, a multiset consisting of $n$ elements always has $2^n$ distinct subsets regardless of whether some of its elements are equal.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$, where $n$ is the number of elements in $A$ ($1\le k\le n\le 600$).</p><p>The second line of input contains $n$ integers $a_1,a_2,\dots,a_n$, describing the elements in $A$ ($-10^9\le a_i\le 10^9$).</p></div><div class="output-specification"><p>Output $\sum\limits_{B\subseteq A} f(B)$ modulo $10^9+7$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$, where $n$ is the number of elements in $A$ ($1\le k\le n\le 600$).</p><p>The second line of input contains $n$ integers $a_1,a_2,\dots,a_n$, describing the elements in $A$ ($-10^9\le a_i\le 10^9$).</p>

## Output

<p>Output $\sum\limits_{B\subseteq A} f(B)$ modulo $10^9+7$.</p>





```input1
3 2
-1 2 4
```




```input2
3 1
1 1 1
```




```input3
10 4
-24 -41 9 -154 -56 14 18 53 -7 120
```




```input4
15 5
0 0 2 -2 2 -2 3 -3 -3 4 5 -4 -4 4 5
```




```output1
10
```




```output2
7
```




```output3
225905161
```




```output4
18119684
```



## Note

<p>Consider the first sample. From the definitions we know that</p><ul> <li> $f(\varnothing)=0$ </li><li> $f(\{-1\})=0$ </li><li> $f(\{2\})=0$ </li><li> $f(\{4\})=0$ </li><li> $f(\{-1,2\})=-2$ </li><li> $f(\{-1,4\})=-4$ </li><li> $f(\{2,4\})=8$ </li><li> $f(\{-1,2,4\})=8$ </li></ul><p>So we should print $(0+0+0+0-2-4+8+8)\bmod (10^9+7)=10$.</p><p>In the second example, note that although the multiset consists of three same values, it still has $8$ distinct subsets: $\varnothing,\{1\},\{1\},\{1\},\{1,1\},\{1,1\},\{1,1\},\{1,1,1\}$.</p>
