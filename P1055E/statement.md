## Description

<div><p>You are a given a list of integers $a_1, a_2, \ldots, a_n$ and $s$ of its segments $[l_j; r_j]$ (where $1 \le l_j \le r_j \le n$).</p><p>You need to select exactly $m$ segments in such a way that the $k$-th order statistic of the multiset of $a_i$, where $i$ is contained in at least one segment, is the smallest possible. If it's impossible to select a set of $m$ segments in such a way that the multiset contains at least $k$ elements, print <span class="tex-font-style-tt">-1</span>.</p><p>The $k$-th order statistic of a multiset is the value of the $k$-th element after sorting the multiset in non-descending order.</p></div><div class="input-specification"><p>The first line contains four integers $n$, $s$, $m$ and $k$ ($1 \le m \le s \le 1500$, $1 \le k \le n \le 1500$)&nbsp;— the size of the list, the number of segments, the number of segments to choose and the statistic number.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— the values of the numbers in the list.</p><p>Each of the next $s$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the endpoints of the segments.</p><p>It is possible that some segments coincide.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the smallest possible $k$-th order statistic, or <span class="tex-font-style-tt">-1</span> if it's impossible to choose segments in a way that the multiset contains at least $k$ elements.</p></div>

## Input

<p>The first line contains four integers $n$, $s$, $m$ and $k$ ($1 \le m \le s \le 1500$, $1 \le k \le n \le 1500$)&nbsp;— the size of the list, the number of segments, the number of segments to choose and the statistic number.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— the values of the numbers in the list.</p><p>Each of the next $s$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the endpoints of the segments.</p><p>It is possible that some segments coincide.</p>

## Output

<p>Print exactly one integer&nbsp;— the smallest possible $k$-th order statistic, or <span class="tex-font-style-tt">-1</span> if it's impossible to choose segments in a way that the multiset contains at least $k$ elements.</p>





```input1
4 3 2 2
3 1 3 2
1 2
2 3
4 4

```




```input2
5 2 1 1
1 2 3 4 5
2 4
1 5

```




```input3
5 3 3 5
5 5 2 1 1
1 2
2 3
3 4

```




```output1
2

```




```output2
1

```




```output3
-1

```



## Note

<p>In the first example, one possible solution is to choose the first and the third segment. Together they will cover three elements of the list (all, except for the third one). This way the $2$-nd order statistic for the covered elements is $2$.</p><p><img class="tex-graphics" src="file://LkSb6Wwo.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
