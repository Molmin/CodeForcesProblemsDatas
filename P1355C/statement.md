## Description

<div><p>Like any unknown mathematician, Yuri has favourite numbers: $A$, $B$, $C$, and $D$, where $A \leq B \leq C \leq D$. Yuri also likes triangles and once he thought: how many non-degenerate triangles with integer sides $x$, $y$, and $z$ exist, such that $A \leq x \leq B \leq y \leq C \leq z \leq D$ holds?</p><p>Yuri is preparing problems for a new contest now, so he is very busy. That's why he asked you to calculate the number of triangles with described property.</p><p>The triangle is called non-degenerate if and only if its vertices are not collinear.</p></div><div class="input-specification"><p>The first line contains four integers: $A$, $B$, $C$ and $D$ ($1 \leq A \leq B \leq C \leq D \leq 5 \cdot 10^5$)&nbsp;— Yuri's favourite numbers.</p></div><div class="output-specification"><p>Print the number of non-degenerate triangles with integer sides $x$, $y$, and $z$ such that the inequality $A \leq x \leq B \leq y \leq C \leq z \leq D$ holds.</p></div>

## Input

<p>The first line contains four integers: $A$, $B$, $C$ and $D$ ($1 \leq A \leq B \leq C \leq D \leq 5 \cdot 10^5$)&nbsp;— Yuri's favourite numbers.</p>

## Output

<p>Print the number of non-degenerate triangles with integer sides $x$, $y$, and $z$ such that the inequality $A \leq x \leq B \leq y \leq C \leq z \leq D$ holds.</p>





```input1
1 2 3 4
```




```input2
1 2 2 5
```




```input3
500000 500000 500000 500000
```




```output1
4
```




```output2
3
```




```output3
1
```



## Note

<p>In the first example Yuri can make up triangles with sides $(1, 3, 3)$, $(2, 2, 3)$, $(2, 3, 3)$ and $(2, 3, 4)$.</p><p>In the second example Yuri can make up triangles with sides $(1, 2, 2)$, $(2, 2, 2)$ and $(2, 2, 3)$.</p><p>In the third example Yuri can make up only one equilateral triangle with sides equal to $5 \cdot 10^5$.</p>
