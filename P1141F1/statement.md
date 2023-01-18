## Description

<div><p><span class="tex-font-style-it">This problem is given in two editions, which differ exclusively in the constraints on the number $n$.</span></p><p>You are given an array of integers $a[1], a[2], \dots, a[n].$ A <span class="tex-font-style-it">block</span> is a sequence of contiguous (consecutive) elements $a[l], a[l+1], \dots, a[r]$ ($1 \le l \le r \le n$). Thus, a block is defined by a pair of indices $(l, r)$.</p><p>Find a set of blocks $(l_1, r_1), (l_2, r_2), \dots, (l_k, r_k)$ such that:</p><ul> <li> They do not intersect (i.e. they are disjoint). Formally, for each pair of blocks $(l_i, r_i)$ and $(l_j, r_j$) where $i \neq j$ either $r_i &lt; l_j$ or $r_j &lt; l_i$. </li><li> For each block the sum of its elements is the same. Formally, $$a[l_1]+a[l_1+1]+\dots+a[r_1]=a[l_2]+a[l_2+1]+\dots+a[r_2]=$$ $$\dots =$$ $$a[l_k]+a[l_k+1]+\dots+a[r_k].$$ </li><li> The number of the blocks in the set is maximum. Formally, there does not exist a set of blocks $(l_1', r_1'), (l_2', r_2'), \dots, (l_{k'}', r_{k'}')$ satisfying the above two requirements with $k' &gt; k$. </li></ul><center> <img class="tex-graphics" src="file://aPqSEPLS.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture corresponds to the first example. Blue boxes illustrate blocks.</span> </center><p>Write a program to find such a set of blocks.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($1 \le n \le 50$) — the length of the given array. The second line contains the sequence of elements $a[1], a[2], \dots, a[n]$ ($-10^5 \le a_i \le 10^5$).</p></div><div class="output-specification"><p>In the first line print the integer $k$ ($1 \le k \le n$). The following $k$ lines should contain blocks, one per line. In each line print a pair of indices $l_i, r_i$ ($1 \le l_i \le r_i \le n$) — the bounds of the $i$-th block. You can print blocks in any order. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains integer $n$ ($1 \le n \le 50$) — the length of the given array. The second line contains the sequence of elements $a[1], a[2], \dots, a[n]$ ($-10^5 \le a_i \le 10^5$).</p>

## Output

<p>In the first line print the integer $k$ ($1 \le k \le n$). The following $k$ lines should contain blocks, one per line. In each line print a pair of indices $l_i, r_i$ ($1 \le l_i \le r_i \le n$) — the bounds of the $i$-th block. You can print blocks in any order. If there are multiple answers, print any of them.</p>





```input1
7
4 1 2 2 1 5 3
```




```input2
11
-5 -4 -3 -2 -1 0 1 2 3 4 5
```




```input3
4
1 1 1 1
```




```output1
3
7 7
2 3
4 5
```




```output2
2
3 4
1 1
```




```output3
4
4 4
1 1
2 2
3 3
```


