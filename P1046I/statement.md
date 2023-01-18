## Description

<div><p>Two friends are travelling through Bubble galaxy. They say "Hello!" via signals to each other if their distance is smaller or equal than $d_1$ and </p><ul>  <li> it's the first time they speak to each other or  </li><li> at some point in time after their last talk their distance was greater than $d_2$. </li></ul><p>We need to calculate how many times friends said "Hello!" to each other. For $N$ moments, you'll have an array of points for each friend representing their positions at that moment. A person can stay in the same position between two moments in time, but if a person made a move we assume this movement as movement with constant speed in constant direction.</p></div><div class="input-specification"><p>The first line contains one integer number $N$ ($2 \leq N \leq 100\,000$) representing number of moments in which we captured positions for two friends.</p><p>The second line contains two integer numbers $d_1$ and $d_2 \ (0 &lt; d_1 &lt; d_2 &lt; 1000)$. </p><p>The next $N$ lines contains four integer numbers $A_x,A_y,B_x,B_y$ ($0 \leq A_x, A_y, B_x, B_y \leq 1000$) representing coordinates of friends A and B in each captured moment.</p></div><div class="output-specification"><p>Output contains one integer number that represents how many times friends will say "Hello!" to each other.</p></div>

## Input

<p>The first line contains one integer number $N$ ($2 \leq N \leq 100\,000$) representing number of moments in which we captured positions for two friends.</p><p>The second line contains two integer numbers $d_1$ and $d_2 \ (0 &lt; d_1 &lt; d_2 &lt; 1000)$. </p><p>The next $N$ lines contains four integer numbers $A_x,A_y,B_x,B_y$ ($0 \leq A_x, A_y, B_x, B_y \leq 1000$) representing coordinates of friends A and B in each captured moment.</p>

## Output

<p>Output contains one integer number that represents how many times friends will say "Hello!" to each other.</p>





```input1
4
2 5
0 0 0 10
5 5 5 6
5 0 10 5
14 7 10 5

```




```output1
2

```



## Note

<p><img class="tex-graphics" src="file://aa1YiZTA.png" style="max-width: 100.0%;max-height: 100.0%;"> Explanation: Friends should send signals 2 times to each other, first time around point $A2$ and $B2$ and second time during A's travel from point $A3$ to $A4$ while B stays in point $B3=B4$. </p>
