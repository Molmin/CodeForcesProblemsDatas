## Description

<div><p>Cirno gives AquaMoon a problem. There are $m$ people numbered from $0$ to $m - 1$. They are standing on a coordinate axis in points with positive integer coordinates. They are facing right (i.e. in the direction of the coordinate increase). At this moment everyone will start running with the constant speed in the direction of coordinate increasing. The initial coordinate of the $i$-th person on the line is $x_i$, and the speed of the $i$-th person is $v_i$. So the coordinate of the $i$-th person at the moment $t$ will be $x_i + t \cdot v_i$.</p><p>Cirno captured the coordinates of $m$ people in $k$ consecutive integer moments from $0$ to $k - 1$. In every moment, the coordinates of $m$ people were recorded in <span class="tex-font-style-bf">arbitrary order</span>.</p><p>To make the problem more funny, Cirno modified one coordinate at the moment $y$ ($0 &lt; y &lt; k-1$) to a <span class="tex-font-style-bf">different</span> integer.</p><p>AquaMoon wants to find the moment $y$ and the original coordinate $p$ before the modification. Actually, she is not a programmer at all. So she wasn't able to solve it. Can you help her?</p></div><div class="input-specification"><p><span class="tex-font-style-bf">This problem is made as interactive. It means, that your solution will read the input, given by the interactor. But the interactor will give you the full input at the beginning and after that, you should print the answer. So you should solve the problem, like as you solve the usual, non-interactive problem because you won't have any interaction process. The only thing you should not forget is to flush the output buffer, after printing the answer. Otherwise, you can get an "Idleness limit exceeded" verdict. Refer to the <a href="https://codeforces.com/blog/entry/45307">interactive problems guide</a> for the detailed information about flushing the output buffer.</span></p><p>The first line contains two integers $m$ and $k$ ($5 \leq m \leq 1000$, $7 \leq k \leq 1000$) — the number of people and the number of recorded moments. </p><p>The next $k$ lines contain captured positions. $i$-th of these lines contains $m$ integers between $1$ and $10^6$ (inclusive), representing positions captured by Cirno at the moment $i-1$.</p><p>The input is guaranteed to be valid (i.e. only one integer was modified to a different value according to the problem statement). Also, it is guaranteed, that $1 \le v_i \le 1000$ for all $1 \leq i \leq m$.</p><p><span class="tex-font-style-bf">Hack format</span>:</p><p>The first line should contain two integers $m$ and $k$ ($5 \leq m \leq 1000$, $7 \leq k \leq 1000$) — the number of people and the number of moments. </p><p>In the second line, there should be $m$ integers $x_0, x_1, \dots,x_{m - 1}$ ($1 \le x_i \le 10^6$), where $x_i$ is the initial coordinate of the $i$-th person.</p><p>In the third line, there should be $m$ integers $v_0, v_1, \dots,v_{m - 1}$ ($1 \le v_i \le 1000$), where $v_i$ is the speed of the $i$-th person. It should be true that $x_i + (k-1) v_i \leq 10^6$ for each $0 \leq i &lt; m$.</p><p>In the next $k$ lines, each line should contain $m$ integers. $i$-th line should contain $m$ distinct integers $p_0, p_1, \ldots, p_{m-1}$ ($0 \leq p_j &lt; m$). The meaning of these numbers: $j$-th integer in the input in the $i$-th moment is the coordinate of the $p_{j}$-th person.</p><p>In the last line, there should be three integers $y$, $i$, $c$. Cirno modified the coordinate of the $i$-th person at the moment $y$ to $c$ ($1 \leq y \leq k-2$, $0 \leq i \leq m - 1$, $1 \leq c \leq 10^6$, $c \neq x_i + y \cdot v_i$).</p></div><div class="output-specification"><p>Print a single line with two integers $y$, $p$ — the moment that contains the modified coordinate and the original coordinate.</p></div>

## Input

<p><span class="tex-font-style-bf">This problem is made as interactive. It means, that your solution will read the input, given by the interactor. But the interactor will give you the full input at the beginning and after that, you should print the answer. So you should solve the problem, like as you solve the usual, non-interactive problem because you won't have any interaction process. The only thing you should not forget is to flush the output buffer, after printing the answer. Otherwise, you can get an "Idleness limit exceeded" verdict. Refer to the <a href="https://codeforces.com/blog/entry/45307">interactive problems guide</a> for the detailed information about flushing the output buffer.</span></p><p>The first line contains two integers $m$ and $k$ ($5 \leq m \leq 1000$, $7 \leq k \leq 1000$) — the number of people and the number of recorded moments. </p><p>The next $k$ lines contain captured positions. $i$-th of these lines contains $m$ integers between $1$ and $10^6$ (inclusive), representing positions captured by Cirno at the moment $i-1$.</p><p>The input is guaranteed to be valid (i.e. only one integer was modified to a different value according to the problem statement). Also, it is guaranteed, that $1 \le v_i \le 1000$ for all $1 \leq i \leq m$.</p><p><span class="tex-font-style-bf">Hack format</span>:</p><p>The first line should contain two integers $m$ and $k$ ($5 \leq m \leq 1000$, $7 \leq k \leq 1000$) — the number of people and the number of moments. </p><p>In the second line, there should be $m$ integers $x_0, x_1, \dots,x_{m - 1}$ ($1 \le x_i \le 10^6$), where $x_i$ is the initial coordinate of the $i$-th person.</p><p>In the third line, there should be $m$ integers $v_0, v_1, \dots,v_{m - 1}$ ($1 \le v_i \le 1000$), where $v_i$ is the speed of the $i$-th person. It should be true that $x_i + (k-1) v_i \leq 10^6$ for each $0 \leq i &lt; m$.</p><p>In the next $k$ lines, each line should contain $m$ integers. $i$-th line should contain $m$ distinct integers $p_0, p_1, \ldots, p_{m-1}$ ($0 \leq p_j &lt; m$). The meaning of these numbers: $j$-th integer in the input in the $i$-th moment is the coordinate of the $p_{j}$-th person.</p><p>In the last line, there should be three integers $y$, $i$, $c$. Cirno modified the coordinate of the $i$-th person at the moment $y$ to $c$ ($1 \leq y \leq k-2$, $0 \leq i \leq m - 1$, $1 \leq c \leq 10^6$, $c \neq x_i + y \cdot v_i$).</p>

## Output

<p>Print a single line with two integers $y$, $p$ — the moment that contains the modified coordinate and the original coordinate.</p>





```input1
5 7
6 9 9 6 9
10 7 10 8 10
11 11 11 10 8
12 12 12 12 9
14 13 12 10 13
11 14 16 14 14
12 15 18 15 15
```




```output1
4 13
```



## Note

<p>In the first test the initial coordinates of people are $9$, $6$, $6$, $9$, $9$ and their speeds are $1$, $2$, $1$, $1$, $1$. So, it's easy to see, that at the moment $4$ one coordinate was modified from $13$ to $12$.</p><p>This is the first test in the hack format:</p><pre class="verbatim"><br>5 7<br>9 6 6 9 9<br>1 2 1 1 1<br>2 3 4 1 0<br>0 2 3 1 4<br>4 3 0 1 2<br>1 3 4 0 2<br>1 4 0 2 3<br>2 4 1 3 0<br>2 4 1 3 0<br>4 0 12<br></pre>
