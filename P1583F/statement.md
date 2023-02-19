## Description

<div><p><span class="tex-font-style-it">Even if you just leave them be, they will fall to pieces all by themselves. So, someone has to protect them, right?</span></p><p>You find yourself playing with Teucer again in the city of Liyue. As you take the eccentric little kid around, you notice something interesting about the structure of the city.</p><p>Liyue can be represented as a directed graph containing $n$ nodes. Nodes are labeled from $1$ to $n$. There is a directed edge from node $a$ to node $b$ if and only if $a &lt; b$.</p><p>A path between nodes $a$ and $b$ is defined as a sequence of edges such that you can start at $a$, travel along all of these edges in the corresponding direction, and end at $b$. The length of a path is defined by the number of edges. A rainbow path of length $x$ is defined as a path in the graph such that there exists at least 2 distinct colors among the set of $x$ edges.</p><p>Teucer's favorite number is $k$. You are curious about the following scenario: If you were to label each edge with a color, what is the minimum number of colors needed to ensure that all paths of length $k$ or longer are rainbow paths?</p><p>Teucer wants to surprise his older brother with a map of Liyue. He also wants to know a valid coloring of edges that uses the minimum number of colors. Please help him with this task!</p></div><div class="input-specification"><p>The only line of input contains two integers $n$ and $k$ ($2 \leq k &lt; n \leq 1000$). </p></div><div class="output-specification"><p>On the first line, output $c$, the minimum colors you need to satisfy the above requirements.</p><p>On the second line, print a valid edge coloring as an array of $\frac{n(n-1)}{2}$ integers ranging from $1$ to $c$. Exactly $c$ distinct colors should exist in the construction. Print the edges in increasing order by the start node first, then by the second node.</p><p>For example, if $n=4$, the edge colors will correspond to this order of edges: ($1$, $2$), ($1$, $3$), ($1$, $4$), ($2$, $3$), ($2$, $4$), ($3$, $4$)</p></div>

## Input

<p>The only line of input contains two integers $n$ and $k$ ($2 \leq k &lt; n \leq 1000$). </p>

## Output

<p>On the first line, output $c$, the minimum colors you need to satisfy the above requirements.</p><p>On the second line, print a valid edge coloring as an array of $\frac{n(n-1)}{2}$ integers ranging from $1$ to $c$. Exactly $c$ distinct colors should exist in the construction. Print the edges in increasing order by the start node first, then by the second node.</p><p>For example, if $n=4$, the edge colors will correspond to this order of edges: ($1$, $2$), ($1$, $3$), ($1$, $4$), ($2$, $3$), ($2$, $4$), ($3$, $4$)</p>





```input1
5 3
```




```input2
5 2
```




```input3
8 7
```




```input4
3 2
```




```output1
2
1 2 2 2 2 2 2 1 1 1
```




```output2
3
3 2 2 1 2 2 1 3 1 1
```




```output3
2
2 2 2 2 2 2 2 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
```




```output4
2
1 2 2
```



## Note

<p>The corresponding construction for the first test case looks like this: </p><center> <img class="tex-graphics" src="file://OZunNTDR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> It is impossible to satisfy the constraints with less than $2$ colors.<p>The corresponding construction for the second test case looks like this: </p><center> <img class="tex-graphics" src="file://D8t4wHzF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> One can show there exists no construction using less than $3$ colors.
