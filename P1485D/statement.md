## Description

<div><p>You are given a matrix $a$ consisting of positive integers. It has $n$ rows and $m$ columns.</p><p>Construct a matrix $b$ consisting of positive integers. It should have the same size as $a$, and the following conditions should be met: </p><ul> <li> $1 \le b_{i,j} \le 10^6$; </li><li> $b_{i,j}$ is a multiple of $a_{i,j}$; </li><li> the absolute value of the difference between numbers in any adjacent pair of cells (two cells that share the same side) in $b$ is equal to $k^4$ for some integer $k \ge 1$ ($k$ is not necessarily the same for all pairs, it is own for each pair). </li></ul><p>We can show that the answer always exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n,m \le 500$).</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer in the $i$-th line is $a_{i,j}$ ($1 \le a_{i,j} \le 16$).</p></div><div class="output-specification"><p>The output should contain $n$ lines each containing $m$ integers. The $j$-th integer in the $i$-th line should be $b_{i,j}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n,m \le 500$).</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer in the $i$-th line is $a_{i,j}$ ($1 \le a_{i,j} \le 16$).</p>

## Output

<p>The output should contain $n$ lines each containing $m$ integers. The $j$-th integer in the $i$-th line should be $b_{i,j}$.</p>





```input1
2 2
1 2
2 3
```




```input2
2 3
16 16 16
16 16 16
```




```input3
2 2
3 11
12 8
```




```output1
1 2
2 3
```




```output2
16 32 48
32 48 64
```




```output3
327 583
408 664
```



## Note

<p>In the first example, the matrix $a$ can be used as the matrix $b$, because the absolute value of the difference between numbers in any adjacent pair of cells is $1 = 1^4$.</p><p>In the third example: </p><ul> <li> $327$ is a multiple of $3$, $583$ is a multiple of $11$, $408$ is a multiple of $12$, $664$ is a multiple of $8$; </li><li> $|408 - 327| = 3^4$, $|583 - 327| = 4^4$, $|664 - 408| = 4^4$, $|664 - 583| = 3^4$. </li></ul>
