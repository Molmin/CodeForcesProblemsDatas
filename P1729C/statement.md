## Description

<div><p>Polycarp was given a row of tiles. Each tile contains one lowercase letter of the Latin alphabet. The entire sequence of tiles forms the string $s$.</p><p>In other words, you are given a string $s$ consisting of lowercase Latin letters.</p><p>Initially, Polycarp is on the <span class="tex-font-style-bf">first</span> tile of the row and wants to get to the <span class="tex-font-style-bf">last</span> tile by jumping on the tiles. Jumping from $i$-th tile to $j$-th tile has a cost equal to $|index(s_i) - index(s_j)|$, where $index(c)$ is the index of the letter $c$ in the alphabet (for example, $index($'<span class="tex-font-style-tt">a</span>'$)=1$, $index($'<span class="tex-font-style-tt">b</span>'$)=2$, ..., $index($'<span class="tex-font-style-tt">z</span>'$)=26$) .</p><p>Polycarp wants to get to the $n$-th tile for the minimum total cost, but at the same time make <span class="tex-font-style-bf">maximum</span> number of jumps.</p><p>In other words, among all possible ways to get to the last tile for the <span class="tex-font-style-bf">minimum</span> total cost, he will choose the one with the <span class="tex-font-style-bf">maximum</span> number of jumps.</p><p>Polycarp can visit each tile <span class="tex-font-style-bf">at most once</span>.</p><p>Polycarp asks you to help&nbsp;— print the sequence of indices of string $s$ on which he should jump.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>Each test case is given by the string $s$ ($2 \le |s| \le 2 \cdot 10^5$), where $|s|$&nbsp;— is the length of string $s$. The string $s$ consists of lowercase Latin letters.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>The answer to each test case consists of two lines.</p><p>In the first line print two integers $cost$, $m$, where $cost$ is the minimum total cost of the path, and $m$ is the maximum number of visited tiles Polycarp can make to get to $n$-th tiles for the minimum total cost $cost$ (i.e. the number of jumps is $m-1$).</p><p>In the next line print $m$ different numbers $j_1, j_2, \dots, j_m$ ($1 \le j_i \le |s|$)&nbsp;— the sequence of indices of the tiles Polycarp will jump on. The first number in the sequence must be $1$ (that is, $j_1=1$) and the last number must be the value of $|s|$ (that is, $j_m=|s|$).</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>Each test case is given by the string $s$ ($2 \le |s| \le 2 \cdot 10^5$), where $|s|$&nbsp;— is the length of string $s$. The string $s$ consists of lowercase Latin letters.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>The answer to each test case consists of two lines.</p><p>In the first line print two integers $cost$, $m$, where $cost$ is the minimum total cost of the path, and $m$ is the maximum number of visited tiles Polycarp can make to get to $n$-th tiles for the minimum total cost $cost$ (i.e. the number of jumps is $m-1$).</p><p>In the next line print $m$ different numbers $j_1, j_2, \dots, j_m$ ($1 \le j_i \le |s|$)&nbsp;— the sequence of indices of the tiles Polycarp will jump on. The first number in the sequence must be $1$ (that is, $j_1=1$) and the last number must be the value of $|s|$ (that is, $j_m=|s|$).</p><p>If there are multiple answers, print any of them.</p>





```input1|2,4,6
6
logic
codeforces
bca
aaaaaaaaaaa
adbaadabad
to
```




```output1
9 4
1 4 3 5
16 10
1 8 3 4 9 5 2 6 7 10
1 2
1 3
0 11
1 8 10 4 3 5 7 2 9 6 11
3 10
1 9 5 4 7 3 8 6 2 10
5 2
1 2
```



## Note

<p>In the first test case, the required path corresponds to the picture:</p><center> <img class="tex-graphics" src="file://6uMk3Nwl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In this case, the minimum possible total cost of the path is achieved. Since $index($'<span class="tex-font-style-tt">l</span>'$)=12$, $index($'<span class="tex-font-style-tt">o</span>'$)=15$, $index($'<span class="tex-font-style-tt">g</span>'$)=7$, $index($'<span class="tex-font-style-tt">i</span>'$)=9$, $index($'<span class="tex-font-style-tt">c</span>'$)=3$, then the total cost of the path is $|12-9|+|9-7|+|7-3|=3+2+4=9$.</p>
