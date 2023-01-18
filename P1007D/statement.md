## Description

<div><p>There is a tree with $n$ vertices. There are also $m$ ants living on it. Each ant has its own color. The $i$-th ant has two favorite pairs of vertices: ($a_i, b_i$) and ($c_i, d_i$). You need to tell if it is possible to paint the edges of the tree in $m$ colors so that every ant will be able to walk between vertices from one of its favorite pairs using only edges of his color; if it is possible, you need to print which pair every ant should use.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of vertices.</p><p>Each of the next $n-1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$), meaning that there is an edge between vertices $u_i$ and $v_i$.</p><p>The next line contains a single integer $m$ ($1 \leq m \leq 10^4$)&nbsp;— the number of ants.</p><p>Each of the next $m$ lines contains four integers $a_i$, $b_i$, $c_i$, and $d_i$ ($1 \leq a_i, b_i, c_i, d_i \leq n$, $a_i \neq b_i, c_i \neq d_i$), meaning that pairs ($a_i$, $b_i$) and ($c_i$, $d_i$) are favorite for the $i$-th ant.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes) if the wanted painting is impossible.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Print $m$ lines. On the $i$-th line, print $1$ if the $i$-th ant will use the first pair and $2$ otherwise. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of vertices.</p><p>Each of the next $n-1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$), meaning that there is an edge between vertices $u_i$ and $v_i$.</p><p>The next line contains a single integer $m$ ($1 \leq m \leq 10^4$)&nbsp;— the number of ants.</p><p>Each of the next $m$ lines contains four integers $a_i$, $b_i$, $c_i$, and $d_i$ ($1 \leq a_i, b_i, c_i, d_i \leq n$, $a_i \neq b_i, c_i \neq d_i$), meaning that pairs ($a_i$, $b_i$) and ($c_i$, $d_i$) are favorite for the $i$-th ant.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes) if the wanted painting is impossible.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Print $m$ lines. On the $i$-th line, print $1$ if the $i$-th ant will use the first pair and $2$ otherwise. If there are multiple answers, print any.</p>





```input1
6
1 2
3 1
4 1
5 2
6 2
3
2 6 3 4
1 6 6 5
1 4 5 2

```




```input2
5
1 2
1 3
1 4
1 5
2
2 3 4 5
3 4 5 2

```




```output1
YES
2
1
2

```




```output2
NO

```



## Note

<p>In the sample, the second and the third edge should be painted in the first color, the first and the fifth should be painted in the second color, and the fourth should be painted in the third color.</p>
