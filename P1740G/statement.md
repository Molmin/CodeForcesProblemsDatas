## Description

<div><p>Pak Chanek has an $n \times m$ grid of portals. The portal on the $i$-th row and $j$-th column is denoted as portal $(i,j)$. The portals $(1,1)$ and $(n,m)$ are on the north-west and south-east corner of the grid respectively.</p><p>The portal $(i,j)$ has two settings:</p><ul> <li> <span class="tex-font-style-bf">Type</span> $t_{i,j}$, which is either $0$ or $1$. </li><li> <span class="tex-font-style-bf">Strength</span> $s_{i,j}$, which is an integer between $1$ and $10^9$ inclusive. </li></ul> Each portal has $4$ faces labelled with integers $0,1,2,3$, which correspond to the north, east, south, and west direction respectively.<center> <img class="tex-graphics" src="file://jIgKSLBB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>When a laser enters face $k$ of portal $(i, j)$ with speed $x_\text{in}$, it leaves the portal going out of face $(k+2+t_{i,j}) \bmod 4$ with speed $x_\text{out} = \max(x_\text{in},s_{i,j})$. The portal also has to consume $x_\text{out} - x_\text{in}$ units of <span class="tex-font-style-bf">energy</span>. </p><p>Pak Chanek is very bored today. He will shoot $4nm$ lasers with an initial speed of $1$, one into each face of each portal. Each laser will travel throughout this grid of portals until it moves outside the grid or it has passed through $10^{100}$ portals.</p><p>At the end, Pak Chanek thinks that a portal is <span class="tex-font-style-bf">good</span> if and only if the total energy consumed by that portal modulo $2$ is equal to its type. Given the strength settings of all portals, find a way to assign the type settings of each portal such that the number of good portals is maximised.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1000$) — the number of rows and columns in the grid.</p><p>The $i$-th of the next $n$ lines contains $m$ integers, with the $j$-th integer being $s_{i,j}$ ($1 \leq s_{i,j} \leq 10^9$) — the strength of portal $(i, j)$.</p></div><div class="output-specification"><p>Print $n$ lines with each line containing a string of length $m$ consisting of characters $0$ or $1$ representing the type settings. The $j$-th character in the $i$-th string is the type setting of portal $(i, j)$.</p><p>If there are multiple solutions, you can output any of them. </p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1000$) — the number of rows and columns in the grid.</p><p>The $i$-th of the next $n$ lines contains $m$ integers, with the $j$-th integer being $s_{i,j}$ ($1 \leq s_{i,j} \leq 10^9$) — the strength of portal $(i, j)$.</p>

## Output

<p>Print $n$ lines with each line containing a string of length $m$ consisting of characters $0$ or $1$ representing the type settings. The $j$-th character in the $i$-th string is the type setting of portal $(i, j)$.</p><p>If there are multiple solutions, you can output any of them. </p>





```input1
2 3
8 8 2
6 5 7
```




```input2
1 2
420 69
```




```output1
110
100
```




```output2
10
```



## Note

<p>In the first example, let's consider the laser Pak Chanek shoots into face $1$ of portal $(2, 2)$. The laser travels as follows: </p><ol> <li> The laser enters face $1$ of portal $(2, 2)$ with speed $1$. It leaves the portal going out of face $3$ with speed $5$. Portal $(2, 2)$ consumes $4$ units of energy. </li><li> The laser enters face $1$ of portal $(2, 1)$ with speed $5$. It leaves the portal going out of face $0$ with speed $6$. Portal $(2, 1)$ consumes $1$ units of energy. </li><li> The laser enters face $2$ of portal $(1, 1)$ with speed $6$. It leaves the portal going out of face $1$ with speed $8$. Portal $(1, 1)$ consumes $2$ units of energy. </li><li> The laser enters face $3$ of portal $(1, 2)$ with speed $8$. It leaves the portal going out of face $2$ with speed $8$. Portal $(1, 2)$ consumes $0$ units of energy. </li><li> The laser enters face $0$ of portal $(2, 2)$ with speed $8$. It leaves the portal going out of face $2$ with speed $8$. Portal $(2, 2)$ consumes $0$ units of energy. </li></ol><p>The illustration of the travel of the laser above is as follows.</p><center> <img class="tex-graphics" src="file://s33VXmE0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As an example, consider portal $(2, 3)$. We can calculate that the total energy consumed by that portal in the end will be $32$. Since $32 \bmod 2 = 0$ and $t_{2,3} = 0$, then it is a good portal.</p>
