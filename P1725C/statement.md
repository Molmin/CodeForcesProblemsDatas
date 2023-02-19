## Description

<div><p>Pak Chanek has a mirror in the shape of a circle. There are $N$ lamps on the circumference numbered from $1$ to $N$ in clockwise order. The length of the arc from lamp $i$ to lamp $i+1$ is $D_i$ for $1 \leq i \leq N-1$. Meanwhile, the length of the arc between lamp $N$ and lamp $1$ is $D_N$.</p><p>Pak Chanek wants to colour the lamps with $M$ different colours. Each lamp can be coloured with one of the $M$ colours. However, there cannot be three different lamps such that the colours of the three lamps are the same and the triangle made by considering the three lamps as vertices is a right triangle (triangle with one of its angles being exactly $90$ degrees).</p><p>The following are examples of lamp colouring configurations on the circular mirror.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://dLomZTu7.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://4XABpYZQ.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://wVY4iZsQ.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr><tr><td class="tex-tabular-text-align-center">Figure 1. an example of an incorrect colouring because lamps $1$, $2$, and $3$ form a right triangle</td><td class="tex-tabular-text-align-center">Figure 2. an example of a correct colouring</td><td class="tex-tabular-text-align-center">Figure 3. an example of a correct colouring</td></tr></tbody></table> </center><p>Before colouring the lamps, Pak Chanek wants to know the number of distinct colouring configurations he can make. Count the number of distinct possible lamp colouring configurations, modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $M$ ($1 \le N \le 3 \cdot 10^5$, $2 \le M \le 3 \cdot 10^5$) — the number of lamps in the mirror and the number of different colours used.</p><p>The second line contains $N$ integers $D_1, D_2, \ldots, D_N$ ($1 \le D_i \le 10^9$) — the lengths of the arcs between the lamps in the mirror.</p></div><div class="output-specification"><p>An integer representing the number of possible lamp colouring configurations, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $N$ and $M$ ($1 \le N \le 3 \cdot 10^5$, $2 \le M \le 3 \cdot 10^5$) — the number of lamps in the mirror and the number of different colours used.</p><p>The second line contains $N$ integers $D_1, D_2, \ldots, D_N$ ($1 \le D_i \le 10^9$) — the lengths of the arcs between the lamps in the mirror.</p>

## Output

<p>An integer representing the number of possible lamp colouring configurations, modulo $998\,244\,353$.</p>





```input1
4 2
10 10 6 14
```




```input2
1 2
10
```




```output1
10
```




```output2
2
```



## Note

<p>In the first example, all correct lamp colouring configurations are $[1, 1, 2, 1]$, $[1, 1, 2, 2]$, $[1, 2, 1, 2]$, $[1, 2, 2, 1]$, $[1, 2, 2, 2]$, $[2, 1, 1, 1]$, $[2, 1, 1, 2]$, $[2, 1, 2, 1]$, $[2, 2, 1, 1]$, and $[2, 2, 1, 2]$.</p>
