## Description

<div><p>The Fair Nut got stacked in planar world. He should solve this task to get out.</p><p>You are given $n$ rectangles with vertexes in $(0, 0)$, $(x_i, 0)$, $(x_i, y_i)$, $(0, y_i)$. For each rectangle, you are also given a number $a_i$. Choose some of them that the area of union minus sum of $a_i$ of the chosen ones is maximum.</p><p>It is guaranteed that there are no nested rectangles.</p><p>Nut has no idea how to find the answer, so he asked for your help.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains three integers $x_i$, $y_i$ and $a_i$ ($1 \leq x_i, y_i \leq 10^9$, $0 \leq a_i \leq x_i \cdot y_i$).</p><p>It is guaranteed that there are no nested rectangles.</p></div><div class="output-specification"><p>In a single line print the answer to the problem&nbsp;— the maximum value which you can achieve.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains three integers $x_i$, $y_i$ and $a_i$ ($1 \leq x_i, y_i \leq 10^9$, $0 \leq a_i \leq x_i \cdot y_i$).</p><p>It is guaranteed that there are no nested rectangles.</p>

## Output

<p>In a single line print the answer to the problem&nbsp;— the maximum value which you can achieve.</p>





```input1
3
4 4 8
1 5 0
5 2 10
```




```input2
4
6 2 4
1 6 2
2 4 3
5 3 8
```




```output1
9
```




```output2
10
```



## Note

<p>In the first example, the right answer can be achieved by choosing the first and the second rectangles.</p><p>In the second example, the right answer can also be achieved by choosing the first and the second rectangles.</p>
