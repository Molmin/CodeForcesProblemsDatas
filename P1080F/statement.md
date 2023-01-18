## Description

<div><p>It is a very important day for Katya. She has a test in a programming class. As always, she was given an interesting problem that she solved very fast. Can you solve that problem?</p><p>You are given $n$ ordered segments sets. Each segment can be represented as a pair of two integers $[l, r]$ where $l\leq r$. Each set can contain an arbitrary number of segments (even $0$). It is possible that some segments are equal.</p><p>You are also given $m$ queries, each of them can be represented as four numbers: $a, b, x, y$. For each segment, find out whether it is true that each set $p$ ($a\leq p\leq b$) contains at least one segment $[l, r]$ that lies entirely on the segment $[x, y]$, that is $x\leq l\leq r\leq y$. </p><p>Find out the answer to each query.</p><p>Note that you need to solve this problem <span class="tex-font-style-bf">online</span>. That is, you will get a new query only after you print the answer for the previous query.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ $(1\leq n,m\leq 10^5, 1\leq k\leq 3\cdot10^5)$&nbsp;— the number of sets, queries, and segments respectively.</p><p>Each of the next $k$ lines contains three integers $l$, $r$, and $p$ $(1\leq l\leq r\leq 10^9, 1\leq p\leq n)$&nbsp;— the limits of the segment and the index of a set, to which this segment belongs.</p><p>Each of the next $m$ lines contains four integers $a, b, x, y$ $(1\leq a\leq b\leq n, 1\leq x\leq y\leq 10^9)$&nbsp;— the description of the query.</p></div><div class="output-specification"><p>For each query, print "<span class="tex-font-style-tt">yes</span>" or "<span class="tex-font-style-tt">no</span>" in a new line.</p></div><div><h2>Interaction</h2><p>After printing a query, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ $(1\leq n,m\leq 10^5, 1\leq k\leq 3\cdot10^5)$&nbsp;— the number of sets, queries, and segments respectively.</p><p>Each of the next $k$ lines contains three integers $l$, $r$, and $p$ $(1\leq l\leq r\leq 10^9, 1\leq p\leq n)$&nbsp;— the limits of the segment and the index of a set, to which this segment belongs.</p><p>Each of the next $m$ lines contains four integers $a, b, x, y$ $(1\leq a\leq b\leq n, 1\leq x\leq y\leq 10^9)$&nbsp;— the description of the query.</p>

## Output

<p>For each query, print "<span class="tex-font-style-tt">yes</span>" or "<span class="tex-font-style-tt">no</span>" in a new line.</p>





```input1
5 5 9
3 6 3
1 3 1
2 4 2
1 2 3
4 6 5
2 5 3
7 9 4
2 3 1
4 10 4
1 2 2 3
1 2 2 4
1 3 1 5
2 3 3 6
2 4 2 9
```




```output1
no
yes
yes
no
yes
```



## Note

<p>For the first query, the answer is negative since the second set does not contain a segment that lies on the segment $[2, 3]$.</p><p>In the second query, the first set contains $[2, 3]$, and the second set contains $[2, 4]$.</p><p>In the third query, the first set contains $[2, 3]$, the second set contains $[2, 4]$, and the third set contains $[2, 5]$.</p><p>In the fourth query, the second set does not contain a segment that lies on the segment $[3, 6]$.</p><p>In the fifth query, the second set contains $[2, 4]$, the third set contains $[2, 5]$, and the fourth contains $[7, 9]$.</p>
