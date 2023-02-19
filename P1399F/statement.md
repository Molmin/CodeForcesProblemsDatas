## Description

<div><p>You are given $n$ segments on a coordinate axis $OX$. The $i$-th segment has borders $[l_i; r_i]$. All points $x$, for which $l_i \le x \le r_i$ holds, belong to the $i$-th segment.</p><p>Your task is to choose the <span class="tex-font-style-bf">maximum</span> by size (the number of segments) subset of the given set of segments such that each pair of segments in this subset either non-intersecting or one of them lies inside the other one.</p><p>Two segments $[l_i; r_i]$ and $[l_j; r_j]$ are non-intersecting if they have <span class="tex-font-style-bf">no common points</span>. For example, segments $[1; 2]$ and $[3; 4]$, $[1; 3]$ and $[5; 5]$ are non-intersecting, while segments $[1; 2]$ and $[2; 3]$, $[1; 2]$ and $[2; 2]$ are intersecting.</p><p>The segment $[l_i; r_i]$ lies inside the segment $[l_j; r_j]$ if $l_j \le l_i$ and $r_i \le r_j$. For example, segments $[2; 2]$, $[2, 3]$, $[3; 4]$ and $[2; 4]$ lie inside the segment $[2; 4]$, while $[2; 5]$ and $[1; 4]$ are not.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 3000$) — the number of segments. The next $n$ lines describe segments. The $i$-th segment is given as two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 2 \cdot 10^5$), where $l_i$ is the left border of the $i$-th segment and $r_i$ is the right border of the $i$-th segment.</p><p>Additional constraint on the input: there are <span class="tex-font-style-bf">no duplicates</span> in the list of segments.</p><p>It is guaranteed that the sum of $n$ does not exceed $3000$ ($\sum n \le 3000$).</p></div><div class="output-specification"><p>For each test case, print the answer: the <span class="tex-font-style-bf">maximum</span> possible size of the subset of the given set of segments such that each pair of segments in this subset either non-intersecting or one of them lies inside the other one.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 3000$) — the number of segments. The next $n$ lines describe segments. The $i$-th segment is given as two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 2 \cdot 10^5$), where $l_i$ is the left border of the $i$-th segment and $r_i$ is the right border of the $i$-th segment.</p><p>Additional constraint on the input: there are <span class="tex-font-style-bf">no duplicates</span> in the list of segments.</p><p>It is guaranteed that the sum of $n$ does not exceed $3000$ ($\sum n \le 3000$).</p>

## Output

<p>For each test case, print the answer: the <span class="tex-font-style-bf">maximum</span> possible size of the subset of the given set of segments such that each pair of segments in this subset either non-intersecting or one of them lies inside the other one.</p>





```input1
4
4
1 5
2 4
2 3
3 4
5
1 5
2 3
2 5
3 5
2 2
3
1 3
2 4
2 3
7
1 10
2 8
2 5
3 4
4 4
6 8
7 7
```




```output1
3
4
2
7
```


