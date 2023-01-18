## Description

<div><p>Since Sonya has just learned the basics of matrices, she decided to play with them a little bit.</p><p>Sonya imagined a new type of matrices that she called <span class="tex-font-style-it">rhombic matrices</span>. These matrices have exactly one zero, while all other cells have the Manhattan distance to the cell containing the zero. The cells with equal numbers have the form of a rhombus, that is why Sonya called this type so.</p><p>The Manhattan distance between two cells ($x_1$, $y_1$) and ($x_2$, $y_2$) is defined as $|x_1 - x_2| + |y_1 - y_2|$. For example, the Manhattan distance between the cells $(5, 2)$ and $(7, 1)$ equals to $|5-7|+|2-1|=3$.</p><center> <img class="tex-graphics" src="file://BHXfbyyk.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example of <span class="tex-font-style-it">a rhombic matrix</span>.</span> </center><p>Note that <span class="tex-font-style-it">rhombic matrices</span> are uniquely defined by $n$, $m$, and the coordinates of the cell containing the zero.</p><p>She drew a $n\times m$ <span class="tex-font-style-it">rhombic matrix</span>. She believes that you can not recreate the matrix if she gives you only the elements of this matrix in some arbitrary order (i.e., the sequence of $n\cdot m$ numbers). Note that Sonya will not give you $n$ and $m$, so only the sequence of numbers in this matrix will be at your disposal.</p><p>Write a program that finds such an $n\times m$ <span class="tex-font-style-it">rhombic matrix</span> whose elements are the same as the elements in the sequence in some order.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 10^6$)&nbsp;— the number of cells in the matrix.</p><p>The second line contains $t$ integers $a_1, a_2, \ldots, a_t$ ($0\leq a_i&lt; t$)&nbsp;— the values in the cells in arbitrary order.</p></div><div class="output-specification"><p>In the first line, print two positive integers $n$ and $m$ ($n \times m = t$)&nbsp;— the size of the matrix.</p><p>In the second line, print two integers $x$ and $y$ ($1\leq x\leq n$, $1\leq y\leq m$)&nbsp;— the row number and the column number where the cell with $0$ is located.</p><p>If there are multiple possible answers, print any of them. If there is no solution, print the single integer $-1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 10^6$)&nbsp;— the number of cells in the matrix.</p><p>The second line contains $t$ integers $a_1, a_2, \ldots, a_t$ ($0\leq a_i&lt; t$)&nbsp;— the values in the cells in arbitrary order.</p>

## Output

<p>In the first line, print two positive integers $n$ and $m$ ($n \times m = t$)&nbsp;— the size of the matrix.</p><p>In the second line, print two integers $x$ and $y$ ($1\leq x\leq n$, $1\leq y\leq m$)&nbsp;— the row number and the column number where the cell with $0$ is located.</p><p>If there are multiple possible answers, print any of them. If there is no solution, print the single integer $-1$.</p>





```input1
20
1 0 2 3 5 3 2 1 3 2 3 1 4 2 1 4 2 3 2 4

```




```input2
18
2 2 3 2 4 3 3 3 0 2 4 2 1 3 2 1 1 1

```




```input3
6
2 1 0 2 1 2

```




```output1
4 5
2 2

```




```output2
3 6
2 3

```




```output3
-1

```



## Note

<p>You can see the solution to the first example in the legend. You also can choose the cell $(2, 2)$ for the cell where $0$ is located. You also can choose a $5\times 4$ matrix with zero at $(4, 2)$.</p><p>In the second example, there is a $3\times 6$ matrix, where the zero is located at $(2, 3)$ there.</p><p>In the third example, a solution does not exist.</p>
