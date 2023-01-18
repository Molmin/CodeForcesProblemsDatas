## Description

<div><p><span class="tex-font-style-it">This problem is same as the next one, but has smaller constraints</span>.</p><p>Aki is playing a new video game. In the video game, he will control Neko, the giant cat, to fly between planets in the Catniverse.</p><p>There are $n$ planets in the Catniverse, numbered from $1$ to $n$. At the beginning of the game, Aki chooses the planet where Neko is initially located. Then Aki performs $k - 1$ moves, where in each move Neko is moved from the current planet $x$ to some other planet $y$ such that:</p><ul> <li> Planet $y$ is not visited yet. </li><li> $1 \leq y \leq x + m$ (where $m$ is a fixed constant given in the input) </li></ul><p>This way, Neko will visit exactly $k$ different planets. Two ways of visiting planets are called different if there is some index $i$ such that the $i$-th planet visited in the first way is different from the $i$-th planet visited in the second way.</p><p>What is the total number of ways to visit $k$ planets this way? Since the answer can be quite large, print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The only line contains three integers $n$, $k$ and $m$ ($1 \le n \le 10^5$, $1 \le k \le \min(n, 12)$, $1 \le m \le 4$)&nbsp;— the number of planets in the Catniverse, the number of planets Neko needs to visit and the said constant $m$.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the number of different ways Neko can visit exactly $k$ planets. Since the answer can be quite large, print it modulo $10^9 + 7$.</p></div>

## Input

<p>The only line contains three integers $n$, $k$ and $m$ ($1 \le n \le 10^5$, $1 \le k \le \min(n, 12)$, $1 \le m \le 4$)&nbsp;— the number of planets in the Catniverse, the number of planets Neko needs to visit and the said constant $m$.</p>

## Output

<p>Print exactly one integer&nbsp;— the number of different ways Neko can visit exactly $k$ planets. Since the answer can be quite large, print it modulo $10^9 + 7$.</p>





```input1
3 3 1
```




```input2
4 2 1
```




```input3
5 5 4
```




```input4
100 1 2
```




```output1
4
```




```output2
9
```




```output3
120
```




```output4
100
```



## Note

<p>In the first example, there are $4$ ways Neko can visit all the planets:</p><ul> <li> $1 \rightarrow 2 \rightarrow 3$ </li><li> $2 \rightarrow 3 \rightarrow 1$ </li><li> $3 \rightarrow 1 \rightarrow 2$ </li><li> $3 \rightarrow 2 \rightarrow 1$ </li></ul><p>In the second example, there are $9$ ways Neko can visit exactly $2$ planets:</p><ul> <li> $1 \rightarrow 2$ </li><li> $2 \rightarrow 1$ </li><li> $2 \rightarrow 3$ </li><li> $3 \rightarrow 1$ </li><li> $3 \rightarrow 2$ </li><li> $3 \rightarrow 4$ </li><li> $4 \rightarrow 1$ </li><li> $4 \rightarrow 2$ </li><li> $4 \rightarrow 3$ </li></ul><p>In the third example, with $m = 4$, Neko can visit all the planets in any order, so there are $5! = 120$ ways Neko can visit all the planets.</p><p>In the fourth example, Neko only visit exactly $1$ planet (which is also the planet he initially located), and there are $100$ ways to choose the starting planet for Neko.</p>
