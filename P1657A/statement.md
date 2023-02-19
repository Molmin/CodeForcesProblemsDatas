## Description

<div><p>There's a chip in the point $(0, 0)$ of the coordinate plane. In one operation, you can move the chip from some point $(x_1, y_1)$ to some point $(x_2, y_2)$ if the Euclidean distance between these two points is an <span class="tex-font-style-bf">integer</span> (i.e. $\sqrt{(x_1-x_2)^2+(y_1-y_2)^2}$ is integer).</p><p>Your task is to determine the minimum number of operations required to move the chip from the point $(0, 0)$ to the point $(x, y)$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 3000$)&nbsp;— number of test cases.</p><p>The single line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 50$)&nbsp;— the coordinates of the destination point.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum number of operations required to move the chip from the point $(0, 0)$ to the point $(x, y)$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 3000$)&nbsp;— number of test cases.</p><p>The single line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 50$)&nbsp;— the coordinates of the destination point.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum number of operations required to move the chip from the point $(0, 0)$ to the point $(x, y)$.</p>





```input1
3
8 6
0 0
9 15
```




```output1
1
0
2
```



## Note

<p>In the first example, one operation $(0, 0) \rightarrow (8, 6)$ is enough. $\sqrt{(0-8)^2+(0-6)^2}=\sqrt{64+36}=\sqrt{100}=10$ is an integer.</p><p>In the second example, the chip is already at the destination point.</p><p>In the third example, the chip can be moved as follows: $(0, 0) \rightarrow (5, 12) \rightarrow (9, 15)$. $\sqrt{(0-5)^2+(0-12)^2}=\sqrt{25+144}=\sqrt{169}=13$ and $\sqrt{(5-9)^2+(12-15)^2}=\sqrt{16+9}=\sqrt{25}=5$ are integers.</p>
