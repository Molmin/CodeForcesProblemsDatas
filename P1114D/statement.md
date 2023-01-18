## Description

<div><p>You are given a line of $n$ colored squares in a row, numbered from $1$ to $n$ from left to right. The $i$-th square initially has the color $c_i$.</p><p>Let's say, that two squares $i$ and $j$ belong to the same connected component if $c_i = c_j$, and $c_i = c_k$ for all $k$ satisfying $i &lt; k &lt; j$. In other words, all squares on the segment from $i$ to $j$ should have the same color.</p><p>For example, the line $[3, 3, 3]$ has $1$ connected component, while the line $[5, 2, 4, 4]$ has $3$ connected components.</p><p>The game "flood fill" is played on the given line as follows: </p><ul> <li> At the start of the game you pick any starting square (this is not counted as a turn). </li><li> Then, in each game turn, change the color of the connected component containing the starting square to any other color. </li></ul><p>Find the minimum number of turns needed for the entire line to be changed into a single color.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the number of squares.</p><p>The second line contains integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 5000$)&nbsp;— the initial colors of the squares.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of the turns needed.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the number of squares.</p><p>The second line contains integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 5000$)&nbsp;— the initial colors of the squares.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of the turns needed.</p>





```input1
4
5 2 2 1
```




```input2
8
4 5 2 2 1 3 5 5
```




```input3
1
4
```




```output1
2
```




```output2
4
```




```output3
0
```



## Note

<p>In the first example, a possible way to achieve an optimal answer is to pick square with index $2$ as the starting square and then play as follows:</p><ul> <li> $[5, 2, 2, 1]$ </li><li> $[5, 5, 5, 1]$ </li><li> $[1, 1, 1, 1]$ </li></ul><p>In the second example, a possible way to achieve an optimal answer is to pick square with index $5$ as the starting square and then perform recoloring into colors $2, 3, 5, 4$ in that order.</p><p>In the third example, the line already consists of one color only.</p>
