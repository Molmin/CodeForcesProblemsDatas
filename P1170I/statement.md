## Description

<div><p>You are given $n$ segments on the $Ox$ axis. The $i$-th segment is given as a pair $l_i, r_i$, where $l_i$ is the position of the left end of the $i$-th segment and $r_i$ is the position of the right end of the $i$-th segment. Segments may intersect, overlap, or even coincide. A segment is a set of numbers (including floating-point numbers) lying between the segment ends or coinciding with them. Formally, the segment $[l, r]=\{x~|~x \in \Bbb{R},~l \le x \le r\}$.</p><p>Let the <span class="tex-font-style-it">union of segments</span> be the set of all axis points covered by the set of segments. Let's call a subset of the given segments <span class="tex-font-style-bf">good</span> if its <span class="tex-font-style-it">union</span> equals the <span class="tex-font-style-it">union</span> of all $n$ segments.</p><p>Your task is to calculate the number of <span class="tex-font-style-bf">good</span> subsets of the given $n$ segments. Since the answer may be very large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain segments. The $i$-th segment is given as a pair $l_i, r_i$ ($1 \le l_i \le r_i \le 10^9$), where $l_i$ is the left border of the segment and $r_i$ is the right border of the segment. Segments may intersect, overlap, or even coincide.</p></div><div class="output-specification"><p>Print the number of <span class="tex-font-style-bf">good</span> subsets of the given set of segments. Since the answer may be very large, print it modulo $998244353$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain segments. The $i$-th segment is given as a pair $l_i, r_i$ ($1 \le l_i \le r_i \le 10^9$), where $l_i$ is the left border of the segment and $r_i$ is the right border of the segment. Segments may intersect, overlap, or even coincide.</p>

## Output

<p>Print the number of <span class="tex-font-style-bf">good</span> subsets of the given set of segments. Since the answer may be very large, print it modulo $998244353$.</p>





```input1
3
1 1
2 6
1 6
```




```input2
2
3 4
2 5
```




```input3
4
1 2
5 5
2 3
1 3
```




```output1
4
```




```output2
2
```




```output3
5
```


