## Description

<div><p>You are given $n$ segments $[l_1, r_1], [l_2, r_2], \dots, [l_n, r_n]$. Each segment has one of two colors: the $i$-th segment's color is $t_i$.</p><p>Let's call a pair of segments $i$ and $j$ <span class="tex-font-style-it">bad</span> if the following two conditions are met:</p><ul> <li> $t_i \ne t_j$; </li><li> the segments $[l_i, r_i]$ and $[l_j, r_j]$ intersect, embed or touch, i. e. there exists an integer $x$ such that $x \in [l_i, r_i]$ and $x \in [l_j, r_j]$. </li></ul><p>Calculate the maximum number of segments that can be selected from the given ones, so that there is no <span class="tex-font-style-it">bad</span> pair among the selected ones.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— number of segments.</p><p>The next $n$ lines contains three integers $l_i, r_i, t_i$ ($1 \le l_i \le r_i \le 10^9; t_i \in \{1, 2\}$)&nbsp;— description of the $i$-th segment.</p></div><div class="output-specification"><p>Print the maximum number of segments that can be selected, so that there is no <span class="tex-font-style-it">bad</span> pair among the selected segments.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— number of segments.</p><p>The next $n$ lines contains three integers $l_i, r_i, t_i$ ($1 \le l_i \le r_i \le 10^9; t_i \in \{1, 2\}$)&nbsp;— description of the $i$-th segment.</p>

## Output

<p>Print the maximum number of segments that can be selected, so that there is no <span class="tex-font-style-it">bad</span> pair among the selected segments.</p>





```input1
3
1 3 1
4 6 2
2 5 1
```




```input2
5
5 8 1
1 3 2
3 4 2
6 6 1
2 10 2
```




```input3
7
19 20 1
13 15 2
6 11 2
4 10 1
14 17 1
13 13 2
5 9 1
```




```output1
2
```




```output2
4
```




```output3
5
```


