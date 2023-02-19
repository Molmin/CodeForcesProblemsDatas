## Description

<div><p>You're creating a game level for some mobile game. The level should contain some number of cells aligned in a row from left to right and numbered with consecutive integers starting from $1$, and in each cell you can either put a platform or leave it empty.</p><p>In order to pass a level, a player must throw a ball from the left so that it first lands on a platform in the cell $p$, then bounces off it, then bounces off a platform in the cell $(p + k)$, then a platform in the cell $(p + 2k)$, and so on every $k$-th platform until it goes farther than the last cell. If any of these cells has no platform, you can't pass the level with these $p$ and $k$.</p><p>You already have some level pattern $a_1$, $a_2$, $a_3$, ..., $a_n$, where $a_i = 0$ means there is no platform in the cell $i$, and $a_i = 1$ means there is one. You want to modify it so that the level can be passed with given $p$ and $k$. In $x$ seconds you can add a platform in some empty cell. In $y$ seconds you can remove the first cell completely, reducing the number of cells by one, and renumerating the other cells keeping their order. You can't do any other operation. You <span class="tex-font-style-bf">can not</span> reduce the number of cells to less than $p$.</p><center> <img class="tex-graphics" height="113px" src="file://ylN4bLsZ.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> <span class="tex-font-size-small">Illustration for the third example test case. Crosses mark deleted cells. Blue platform is the newly added.</span> </center><p>What is the minimum number of seconds you need to make this level passable with given $p$ and $k$?</p></div><div class="input-specification"><p>The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $p$, and $k$ ($1 \le p \le n \le 10^5$, $1 \le k \le n$)&nbsp;— the number of cells you have, the first cell that should contain a platform, and the period of ball bouncing required.</p><p>The second line of each test case contains a string $a_1 a_2 a_3 \ldots a_n$ ($a_i = 0$ or $a_i = 1$)&nbsp;— the initial pattern written <span class="tex-font-style-bf">without spaces</span>.</p><p>The last line of each test case contains two integers $x$ and $y$ ($1 \le x, y \le 10^4$)&nbsp;— the time required to add a platform and to remove the first cell correspondingly.</p><p>The sum of $n$ over test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— the minimum number of seconds you need to modify the level accordingly.</p><p>It can be shown that it is always possible to make the level passable.</p></div>

## Input

<p>The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $p$, and $k$ ($1 \le p \le n \le 10^5$, $1 \le k \le n$)&nbsp;— the number of cells you have, the first cell that should contain a platform, and the period of ball bouncing required.</p><p>The second line of each test case contains a string $a_1 a_2 a_3 \ldots a_n$ ($a_i = 0$ or $a_i = 1$)&nbsp;— the initial pattern written <span class="tex-font-style-bf">without spaces</span>.</p><p>The last line of each test case contains two integers $x$ and $y$ ($1 \le x, y \le 10^4$)&nbsp;— the time required to add a platform and to remove the first cell correspondingly.</p><p>The sum of $n$ over test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output a single integer&nbsp;— the minimum number of seconds you need to modify the level accordingly.</p><p>It can be shown that it is always possible to make the level passable.</p>





```input1
3
10 3 2
0101010101
2 2
5 4 1
00000
2 10
11 2 3
10110011000
4 3
```




```output1
2
4
10
```



## Note

<p>In the first test case it's best to just remove the first cell, after that all required platforms are in their places: <span class="tex-font-style-tt"><span class="tex-font-style-striked">0</span>10<span class="tex-font-style-bf">1</span>0<span class="tex-font-style-bf">1</span>0<span class="tex-font-style-bf">1</span>0<span class="tex-font-style-bf">1</span></span>. The stroked out digit is removed, the bold ones are where platforms should be located. The time required is $y = 2$.</p><p>In the second test case it's best to add a platform to both cells $4$ and $5$: <span class="tex-font-style-tt">000<span class="tex-font-style-bf">00</span></span> $\to$ <span class="tex-font-style-tt">000<span class="tex-font-style-bf">11</span></span>. The time required is $x \cdot 2 = 4$.</p><p>In the third test case it's best to to remove the first cell twice and then add a platform to the cell which was initially $10$-th: <span class="tex-font-style-tt"><span class="tex-font-style-striked">10</span>1<span class="tex-font-style-bf">1</span>00<span class="tex-font-style-bf">1</span>10<span class="tex-font-style-bf">0</span>0</span> $\to$ <span class="tex-font-style-tt"><span class="tex-font-style-striked">10</span>1<span class="tex-font-style-bf">1</span>00<span class="tex-font-style-bf">1</span>10<span class="tex-font-style-bf">1</span>0</span>. The time required is $y \cdot 2 + x = 10$.</p>
