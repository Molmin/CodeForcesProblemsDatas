## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$ of $n$ integers. Consider $S$ as a set of segments satisfying the following conditions.</p><ul> <li> Each element of $S$ should be in form $[x, y]$, where $x$ and $y$ are integers between $1$ and $n$, inclusive, and $x \leq y$. </li><li> No two segments in $S$ intersect with each other. Two segments $[a, b]$ and $[c, d]$ intersect if and only if there exists an integer $x$ such that $a \leq x \leq b$ and $c \leq x \leq d$. </li><li> For each $[x, y]$ in $S$, $a_x+a_{x+1}+ \ldots +a_y \geq 0$. </li></ul><p>The length of the segment $[x, y]$ is defined as $y-x+1$. $f(S)$ is defined as the sum of the lengths of every element in $S$. In a formal way, $f(S) = \sum_{[x, y] \in S} (y - x + 1)$. Note that if $S$ is empty, $f(S)$ is $0$.</p><p>What is the maximum $f(S)$ among all possible $S$?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The next line is followed by $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p></div><div class="output-specification"><p>Print a single integer, the maximum $f(S)$ among every possible $S$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The next line is followed by $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p>

## Output

<p>Print a single integer, the maximum $f(S)$ among every possible $S$.</p>





```input1
5
3 -3 -2 5 -4
```




```input2
10
5 -2 -4 -6 2 3 -6 5 3 -2
```




```input3
4
-1 -2 -3 -4
```




```output1
4
```




```output2
9
```




```output3
0
```



## Note

<p>In the first example, $S=\{[1, 2], [4, 5]\}$ can be a possible $S$ because $a_1+a_2=0$ and $a_4+a_5=1$. $S=\{[1, 4]\}$ can also be a possible solution.</p><p>Since there does not exist any $S$ that satisfies $f(S) &gt; 4$, the answer is $4$.</p><p>In the second example, $S=\{[1, 9]\}$ is the only set that satisfies $f(S)=9$. Since every possible $S$ satisfies $f(S) \leq 9$, the answer is $9$.</p><p>In the third example, $S$ can only be an empty set, so the answer is $0$.</p>
