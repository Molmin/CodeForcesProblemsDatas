## Description

<div><p><span class="tex-font-style-it">Pink Floyd are pulling a prank on Roger Waters. They know he doesn't like <a href="https://www.youtube.com/watch?v=YR5ApYxkU-U">walls</a>, he wants to be able to walk freely, so they are blocking him from exiting his room which can be seen as a grid.</span></p><p>Roger Waters has a square grid of size $n\times n$ and he wants to traverse his grid from the upper left ($1,1$) corner to the lower right corner ($n,n$). Waters can move from a square to any other square adjacent by a side, as long as he is still in the grid. Also except for the cells ($1,1$) and ($n,n$) every cell has a value $0$ or $1$ in it.</p><p>Before starting his traversal he will pick either a $0$ or a $1$ and will be able to only go to cells values in which are equal to the digit he chose. The starting and finishing cells ($1,1$) and ($n,n$) are exempt from this rule, he may go through them regardless of picked digit. Because of this the cell ($1,1$) takes value the letter '<span class="tex-font-style-tt">S</span>' and the cell ($n,n$) takes value the letter '<span class="tex-font-style-tt">F</span>'.</p><p>For example, in the first example test case, he can go from ($1, 1$) to ($n, n$) by using the zeroes on this path: ($1, 1$), ($2, 1$), ($2, 2$), ($2, 3$), ($3, 3$), ($3, 4$), ($4, 4$)</p><p>The rest of the band (Pink Floyd) wants Waters to not be able to do his traversal, so while he is not looking they will <span class="tex-font-style-bf">invert at most two cells</span> in the grid (from $0$ to $1$ or vice versa). They are afraid they will not be quick enough and asked for your help in choosing the cells. <span class="tex-font-style-bf"> Note that you cannot invert cells $(1, 1)$ and $(n, n)$</span>.</p><p>We can show that there always exists a solution for the given constraints.</p><p>Also note that Waters will pick his digit of the traversal after the band has changed his grid, so he must not be able to reach ($n,n$) no matter what digit he picks.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). Description of the test cases follows.</p><p>The first line of each test case contains one integers $n$ ($3 \le n \le 200$).</p><p>The following $n$ lines of each test case contain the binary grid, square ($1, 1$) being colored in '<span class="tex-font-style-tt">S</span>' and square ($n, n$) being colored in '<span class="tex-font-style-tt">F</span>'.</p><p>The sum of values of $n$ doesn't exceed $200$.</p></div><div class="output-specification"><p>For each test case output on the first line an integer $c$ ($0 \le c \le 2$) &nbsp;— the number of inverted cells.</p><p>In $i$-th of the following $c$ lines, print the coordinates of the $i$-th cell you inverted. You may not invert the same cell twice. <span class="tex-font-style-bf"> Note that you cannot invert cells $(1, 1)$ and $(n, n)$</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). Description of the test cases follows.</p><p>The first line of each test case contains one integers $n$ ($3 \le n \le 200$).</p><p>The following $n$ lines of each test case contain the binary grid, square ($1, 1$) being colored in '<span class="tex-font-style-tt">S</span>' and square ($n, n$) being colored in '<span class="tex-font-style-tt">F</span>'.</p><p>The sum of values of $n$ doesn't exceed $200$.</p>

## Output

<p>For each test case output on the first line an integer $c$ ($0 \le c \le 2$) &nbsp;— the number of inverted cells.</p><p>In $i$-th of the following $c$ lines, print the coordinates of the $i$-th cell you inverted. You may not invert the same cell twice. <span class="tex-font-style-bf"> Note that you cannot invert cells $(1, 1)$ and $(n, n)$</span>.</p>





```input1
3
4
S010
0001
1000
111F
3
S10
101
01F
5
S0101
00000
01111
11111
0001F
```




```output1
1
3 4
2
1 2
2 1
0
```



## Note

<p>For the first test case, after inverting the cell, we get the following grid:</p><pre class="verbatim"><br>S010<br>0001<br>1001<br>111F<br></pre>
