## Description

<div><p>Sonya likes ice cream very much. She eats it even during programming competitions. That is why the girl decided that she wants to open her own ice cream shops.</p><p>Sonya lives in a city with $n$ junctions and $n-1$ streets between them. All streets are two-way and connect two junctions. It is possible to travel from any junction to any other using one or more streets. City Hall allows opening shops only on junctions. The girl cannot open shops in the middle of streets. </p><p>Sonya has exactly $k$ friends whom she can trust. If she opens a shop, one of her friends has to work there and not to allow anybody to eat an ice cream not paying for it. Since Sonya does not want to skip an important competition, she will not work in shops personally.</p><p>Sonya wants all her ice cream shops to form a simple path of the length $r$ ($1 \le r \le k$), i.e. to be located in different junctions $f_1, f_2, \dots, f_r$ and there is street between $f_i$ and $f_{i+1}$ for each $i$ from $1$ to $r-1$.</p><p>The girl takes care of potential buyers, so she also wants to minimize the maximum distance between the junctions to the nearest ice cream shop. The distance between two junctions $a$ and $b$ is equal to the sum of all the street lengths that you need to pass to get from the junction $a$ to the junction $b$. So Sonya wants to <span class="tex-font-style-it">minimize</span></p><p>$$\max_{a} \min_{1 \le i \le r} d_{a,f_i}$$</p><p>where $a$ takes a value of all possible $n$ junctions, $f_i$&nbsp;— the junction where the $i$-th Sonya's shop is located, and $d_{x,y}$&nbsp;— the distance between the junctions $x$ and $y$.</p><p>Sonya is not sure that she can find the optimal shops locations, that is why she is asking you to help her to open not more than $k$ shops that will form a simple path and the maximum distance between any junction and the nearest shop would be minimal. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1\leq k\leq n\leq 10^5$)&nbsp;— the number of junctions and friends respectively.</p><p>Each of the next $n-1$ lines contains three integers $u_i$, $v_i$, and $d_i$ ($1\leq u_i, v_i\leq n$, $v_i\neq u_i$, $1\leq d\leq 10^4$)&nbsp;— junctions that are connected by a street and the length of this street. It is guaranteed that each pair of junctions is connected by at most one street. It is guaranteed that you can get from any junctions to any other.</p></div><div class="output-specification"><p>Print one number&nbsp;— the minimal possible maximum distance that you need to pass to get from any junction to the nearest ice cream shop. Sonya's shops must form a simple path and the number of shops must be at most $k$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1\leq k\leq n\leq 10^5$)&nbsp;— the number of junctions and friends respectively.</p><p>Each of the next $n-1$ lines contains three integers $u_i$, $v_i$, and $d_i$ ($1\leq u_i, v_i\leq n$, $v_i\neq u_i$, $1\leq d\leq 10^4$)&nbsp;— junctions that are connected by a street and the length of this street. It is guaranteed that each pair of junctions is connected by at most one street. It is guaranteed that you can get from any junctions to any other.</p>

## Output

<p>Print one number&nbsp;— the minimal possible maximum distance that you need to pass to get from any junction to the nearest ice cream shop. Sonya's shops must form a simple path and the number of shops must be at most $k$.</p>





```input1
6 2
1 2 3
2 3 4
4 5 2
4 6 3
2 4 6

```




```input2
10 3
1 2 5
5 7 2
3 2 6
10 6 3
3 8 1
6 4 2
4 1 6
6 9 4
5 2 5

```




```output1
4

```




```output2
7

```



## Note

<p>In the first example, you can choose the path 2-4, so the answer will be 4.</p><center> <img class="tex-graphics" src="file://ga2unwOp.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The first example.</span> </center><p>In the second example, you can choose the path 4-1-2, so the answer will be 7.</p><center> <img class="tex-graphics" src="file://hZpBCmgn.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The second example.</span> </center>
