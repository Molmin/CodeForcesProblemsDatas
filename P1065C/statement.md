## Description

<div><p>There is a toy building consisting of $n$ towers. Each tower consists of several cubes standing on each other. The $i$-th tower consists of $h_i$ cubes, so it has height $h_i$.</p><p>Let's define operation <span class="tex-font-style-it">slice</span> on some height $H$ as following: for each tower $i$, if its height is greater than $H$, then remove some top cubes to make tower's height equal to $H$. Cost of one "slice" equals to the total number of removed cubes from all towers.</p><p>Let's name slice as <span class="tex-font-style-it">good</span> one if its cost is lower or equal to $k$ ($k \ge n$).</p><center> <img class="tex-graphics" src="file://xnAcFXkH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Calculate the minimum number of good slices you have to do to make all towers have the same height. Of course, it is always possible to make it so.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $n \le k \le 10^9$) — the number of towers and the restriction on slices, respectively.</p><p>The second line contains $n$ space separated integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 2 \cdot 10^5$) — the initial heights of towers.</p></div><div class="output-specification"><p>Print one integer — the minimum number of good slices you have to do to make all towers have the same heigth.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $n \le k \le 10^9$) — the number of towers and the restriction on slices, respectively.</p><p>The second line contains $n$ space separated integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 2 \cdot 10^5$) — the initial heights of towers.</p>

## Output

<p>Print one integer — the minimum number of good slices you have to do to make all towers have the same heigth.</p>





```input1
5 5
3 1 2 2 4

```




```input2
4 5
2 3 4 5

```




```output1
2

```




```output2
2

```



## Note

<p>In the first example it's optimal to make $2$ slices. The first slice is on height $2$ (its cost is $3$), and the second one is on height $1$ (its cost is $4$).</p>
