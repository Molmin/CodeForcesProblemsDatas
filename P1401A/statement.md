## Description

<div><p>We have a point $A$ with coordinate $x = n$ on $OX$-axis. We'd like to find an <span class="tex-font-style-it">integer point</span> $B$ (also on $OX$-axis), such that the <span class="tex-font-style-it">absolute difference</span> between the distance from $O$ to $B$ and the distance from $A$ to $B$ is equal to $k$.</p><center> <img class="tex-graphics" src="file://GfX0nOME.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The description of the first test case.</span> </center><p>Since sometimes it's impossible to find such point $B$, we can, in one step, increase or decrease the coordinate of $A$ by $1$. What is the minimum number of steps we should do to make such point $B$ exist?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 6000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains two integers $n$ and $k$ ($0 \le n, k \le 10^6$)&nbsp;— the initial position of point $A$ and desirable absolute difference.</p></div><div class="output-specification"><p>For each test case, print the minimum number of steps to make point $B$ exist.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 6000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains two integers $n$ and $k$ ($0 \le n, k \le 10^6$)&nbsp;— the initial position of point $A$ and desirable absolute difference.</p>

## Output

<p>For each test case, print the minimum number of steps to make point $B$ exist.</p>





```input1
6
4 0
5 8
0 1000000
0 0
1 0
1000000 1000000
```




```output1
0
3
1000000
0
1
0
```



## Note

<p>In the first test case (picture above), if we set the coordinate of $B$ as $2$ then the absolute difference will be equal to $|(2 - 0) - (4 - 2)| = 0$ and we don't have to move $A$. So the answer is $0$.</p><p>In the second test case, we can increase the coordinate of $A$ by $3$ and set the coordinate of $B$ as $0$ or $8$. The absolute difference will be equal to $|8 - 0| = 8$, so the answer is $3$.</p><center> <img class="tex-graphics" src="file://t40yENVF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
