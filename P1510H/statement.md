## Description

<div><p>You are given a set of $n$ segments on a line $[L_i; R_i]$. All $2n$ segment endpoints are pairwise distinct integers.</p><p>The set is <span class="tex-font-style-underline">laminar</span>&nbsp;— any two segments are either disjoint or one of them contains the other.</p><p>Choose a non-empty subsegment $[l_i, r_i]$ with integer endpoints in each segment ($L_i \le l_i &lt; r_i \le R_i$) in such a way that no two subsegments intersect (they are allowed to have common endpoints though) and the sum of their lengths ($\sum_{i=1}^n r_i - l_i$) is maximized.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^3$)&nbsp;— the number of segments.</p><p>The $i$-th of the next $n$ lines contains two integers $L_i$ and $R_i$ ($0 \le L_i &lt; R_i \le 10^9$)&nbsp;— the endpoints of the $i$-th segment.</p><p>All the given $2n$ segment endpoints are distinct. The set of segments is laminar.</p></div><div class="output-specification"><p>On the first line, output the maximum possible sum of subsegment lengths.</p><p>On the $i$-th of the next $n$ lines, output two integers $l_i$ and $r_i$ ($L_i \le l_i &lt; r_i \le R_i$), denoting the chosen subsegment of the $i$-th segment.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^3$)&nbsp;— the number of segments.</p><p>The $i$-th of the next $n$ lines contains two integers $L_i$ and $R_i$ ($0 \le L_i &lt; R_i \le 10^9$)&nbsp;— the endpoints of the $i$-th segment.</p><p>All the given $2n$ segment endpoints are distinct. The set of segments is laminar.</p>

## Output

<p>On the first line, output the maximum possible sum of subsegment lengths.</p><p>On the $i$-th of the next $n$ lines, output two integers $l_i$ and $r_i$ ($L_i \le l_i &lt; r_i \le R_i$), denoting the chosen subsegment of the $i$-th segment.</p>





```input1
4
1 10
2 3
5 9
6 7
```




```output1
7
3 6
2 3
7 9
6 7
```



## Note

<p>The example input and the example output are illustrated below.   <img class="tex-graphics" src="file://iBUqn2GN.png" style="max-width: 100.0%;max-height: 100.0%;">     <img class="tex-graphics" src="file://nbethlxv.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
