## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is constraints</span>.</p><p>You are given $n$ segments on the coordinate axis $OX$. Segments can intersect, lie inside each other and even coincide. The $i$-th segment is $[l_i; r_i]$ ($l_i \le r_i$) and it covers all integer points $j$ such that $l_i \le j \le r_i$.</p><p>The integer point is called <span class="tex-font-style-bf">bad</span> if it is covered by <span class="tex-font-style-bf">strictly more</span> than $k$ segments.</p><p>Your task is to remove the minimum number of segments so that there are no <span class="tex-font-style-bf">bad</span> points at all.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 200$) — the number of segments and the maximum number of segments by which each integer point can be covered.</p><p>The next $n$ lines contain segments. The $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 200$) — the endpoints of the $i$-th segment.</p></div><div class="output-specification"><p>In the first line print one integer $m$ ($0 \le m \le n$) — the minimum number of segments you need to remove so that there are no <span class="tex-font-style-bf">bad</span> points.</p><p>In the second line print $m$ <span class="tex-font-style-bf">distinct</span> integers $p_1, p_2, \dots, p_m$ ($1 \le p_i \le n$) — indices of segments you remove in any order. If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 200$) — the number of segments and the maximum number of segments by which each integer point can be covered.</p><p>The next $n$ lines contain segments. The $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 200$) — the endpoints of the $i$-th segment.</p>

## Output

<p>In the first line print one integer $m$ ($0 \le m \le n$) — the minimum number of segments you need to remove so that there are no <span class="tex-font-style-bf">bad</span> points.</p><p>In the second line print $m$ <span class="tex-font-style-bf">distinct</span> integers $p_1, p_2, \dots, p_m$ ($1 \le p_i \le n$) — indices of segments you remove in any order. If there are multiple answers, you can print any of them.</p>





```input1
7 2
11 11
9 11
7 8
8 9
7 8
9 11
7 9
```




```input2
5 1
29 30
30 30
29 29
28 30
30 30
```




```input3
6 1
2 3
3 3
2 3
2 2
2 3
2 3
```




```output1
3
1 4 7
```




```output2
3
1 2 4
```




```output3
4
1 3 5 6
```


