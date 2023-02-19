## Description

<div><p>Ira is developing a computer game. This game features randomized generation and difficulty of levels. To achieve randomized difficulty, some enemies in each level are randomly replaced with stronger ones.</p><p>To describe how do the levels in the game look, let's introduce a coordinate system in such a way that $Ox$ axis goes from left to right, and $Oy$ axis goes from bottom to top. A level is a rectangle with opposite corners in points $(0, 0)$ and $(a, b)$. Each enemy's position is a point in this rectangle.</p><p>As for now, Ira has implemented one type of enemy in the game, in two different versions&nbsp;— basic and upgraded. Both versions of enemies Ira has implemented fire laser rays in several directions:</p><ul> <li> basic enemies fire four laser rays in four directions: to the right (in the same direction as the vector $(1, 0)$), to the left (in the same direction as the vector $(-1, 0)$), up (in the same direction as the vector $(0, 1)$), and down (in the same direction as the vector $(0, -1)$); </li><li> upgraded enemies fire eight laser rays in eight directions: four directions listed for basic enemies, and four directions corresponding to vectors $(1, 1)$, $(1, -1)$, $(-1, 1)$, $(-1, -1)$. </li></ul><p>Laser rays pass through enemies and are blocked only by the borders of the level (sides of the rectangle that denotes the level). Enemies are unaffected by lasers.</p><p>The level Ira is working on has $n$ enemies. The $i$-th enemy is in the point $(x_i, y_i)$, and it has a probability of $p_i$ to be upgraded (it's either upgraded with probability $p_i$, or basic with probability $1-p_i$). All these events are independent.</p><p>Ira wants to estimate the expected difficulty. She considers that a good way to evaluate the difficulty of the level is to count the number of parts in which the level is divided by the laser rays. So, she wants to calculate the expected number of these parts.</p><p>Help her to do the evaluation of the level!</p></div><div class="input-specification"><p>The first line contains three integers $n$, $a$ and $b$ ($1 \le n \le 100$; $2 \le a, b \le 100$)&nbsp;— the number of enemies in the level and the dimensions of the level.</p><p>Then $n$ lines follow, the $i$-th of them contains three integers $x_i$, $y_i$ and $p'_i$ ($1 \le x_i \le a - 1$; $1 \le y_i \le b - 1$; $1 \le p'_i \le 999999$), meaning that the $i$-th enemy is located at $(x_i, y_i)$ and has a probability of $\frac{p'_i}{10^6}$ to be upgraded.</p><p>No two enemies are located in the same point.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the expected number of parts in which the lasers divide the level, taken modulo $998244353$ (i. e. let the expected number of parts be $\frac{x}{y}$ as an irreducible fraction; you have to print $x \cdot y^{-1} \bmod 998244353$, where $y^{-1}$ is a number such that $y \cdot y^{-1} \bmod 998244353 = 1$).</p></div>

## Input

<p>The first line contains three integers $n$, $a$ and $b$ ($1 \le n \le 100$; $2 \le a, b \le 100$)&nbsp;— the number of enemies in the level and the dimensions of the level.</p><p>Then $n$ lines follow, the $i$-th of them contains three integers $x_i$, $y_i$ and $p'_i$ ($1 \le x_i \le a - 1$; $1 \le y_i \le b - 1$; $1 \le p'_i \le 999999$), meaning that the $i$-th enemy is located at $(x_i, y_i)$ and has a probability of $\frac{p'_i}{10^6}$ to be upgraded.</p><p>No two enemies are located in the same point.</p>

## Output

<p>Print one integer&nbsp;— the expected number of parts in which the lasers divide the level, taken modulo $998244353$ (i. e. let the expected number of parts be $\frac{x}{y}$ as an irreducible fraction; you have to print $x \cdot y^{-1} \bmod 998244353$, where $y^{-1}$ is a number such that $y \cdot y^{-1} \bmod 998244353 = 1$).</p>





```input1
1 2 2
1 1 500000
```




```input2
2 3 2
1 1 500000
2 1 500000
```




```output1
6
```




```output2
499122187
```



## Note

<p>Explanation to the first example:</p><p>With probability $\frac{1}{2}$, the only enemy is not upgraded and the level looks like this ($4$ parts):</p><center> <img class="tex-graphics" src="file://AO4FZzqz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>With probability $\frac{1}{2}$, the only enemy is upgraded and the level looks like this ($8$ parts):</p><center> <img class="tex-graphics" src="file://peFRBwFN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>So, the expected number of parts is $4 \cdot \frac{1}{2} + 8 \cdot \frac{1}{2} = 6$.</p>
