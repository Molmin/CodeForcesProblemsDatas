## Description

<div><p>Major Ram is being chased by his arch enemy Raghav. Ram must reach the top of the building to escape via helicopter. The building, however, is on fire. Ram must choose the optimal path to reach the top of the building to lose the minimum amount of health.</p><p>The building consists of $n$ floors, each with $m$ rooms each. Let $(i, j)$ represent the $j$-th room on the $i$-th floor. Additionally, there are $k$ ladders installed. The $i$-th ladder allows Ram to travel from $(a_i, b_i)$ to $(c_i, d_i)$, but <span class="tex-font-style-bf">not in the other direction</span>. Ram also gains $h_i$ health points if he uses the ladder $i$. <span class="tex-font-style-bf">It is guaranteed $a_i &lt; c_i$ for all ladders.</span></p><p>If Ram is on the $i$-th floor, he can move either left or right. Travelling across floors, however, is treacherous. If Ram travels from $(i, j)$ to $(i, k)$, he loses $|j-k| \cdot x_i$ health points.</p><p>Ram enters the building at $(1, 1)$ while his helicopter is waiting at $(n, m)$. What is the minimum amount of health Ram loses if he takes the most optimal path? Note this answer may be negative (in which case he gains health). Output "<span class="tex-font-style-tt">NO ESCAPE</span>" if no matter what path Ram takes, he cannot escape the clutches of Raghav.</p><center> <img class="tex-graphics" src="file://yKpDZ0a9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line of input contains $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case consists of $3$ integers $n, m, k$ ($2 \leq n, m \leq 10^5$; $1 \leq k \leq 10^5$)&nbsp;— the number of floors, the number of rooms on each floor and the number of ladders respectively.</p><p>The second line of a test case consists of $n$ integers $x_1, x_2, \dots, x_n$ ($1 \leq x_i \leq 10^6$).</p><p>The next $k$ lines describe the ladders. Ladder $i$ is denoted by $a_i, b_i, c_i, d_i, h_i$ ($1 \leq a_i &lt; c_i \leq n$; $1 \leq b_i, d_i \leq m$; $1 \leq h_i \leq 10^6$) &nbsp;— the rooms it connects and the health points gained from using it.</p><p><span class="tex-font-style-bf">It is guaranteed $a_i &lt; c_i$ for all ladders</span> and there is <span class="tex-font-style-bf">at most</span> one ladder between any 2 rooms in the building.</p><p>The sum of $n$, the sum of $m$, and the sum of $k$ over all test cases do not exceed $10^5$.</p></div><div class="output-specification"><p>Output the minimum health Ram loses on the optimal path from $(1, 1)$ to $(n, m)$. If Ram cannot escape the clutches of Raghav regardless of the path he takes, output "<span class="tex-font-style-tt">NO ESCAPE</span>" (all uppercase, without quotes).</p></div>

## Input

<p>The first line of input contains $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case consists of $3$ integers $n, m, k$ ($2 \leq n, m \leq 10^5$; $1 \leq k \leq 10^5$)&nbsp;— the number of floors, the number of rooms on each floor and the number of ladders respectively.</p><p>The second line of a test case consists of $n$ integers $x_1, x_2, \dots, x_n$ ($1 \leq x_i \leq 10^6$).</p><p>The next $k$ lines describe the ladders. Ladder $i$ is denoted by $a_i, b_i, c_i, d_i, h_i$ ($1 \leq a_i &lt; c_i \leq n$; $1 \leq b_i, d_i \leq m$; $1 \leq h_i \leq 10^6$) &nbsp;— the rooms it connects and the health points gained from using it.</p><p><span class="tex-font-style-bf">It is guaranteed $a_i &lt; c_i$ for all ladders</span> and there is <span class="tex-font-style-bf">at most</span> one ladder between any 2 rooms in the building.</p><p>The sum of $n$, the sum of $m$, and the sum of $k$ over all test cases do not exceed $10^5$.</p>

## Output

<p>Output the minimum health Ram loses on the optimal path from $(1, 1)$ to $(n, m)$. If Ram cannot escape the clutches of Raghav regardless of the path he takes, output "<span class="tex-font-style-tt">NO ESCAPE</span>" (all uppercase, without quotes).</p>





```input1
4
5 3 3
5 17 8 1 4
1 3 3 3 4
3 1 5 2 5
3 2 5 1 6
6 3 3
5 17 8 1 4 2
1 3 3 3 4
3 1 5 2 5
3 2 5 1 6
5 3 1
5 17 8 1 4
1 3 5 3 100
5 5 5
3 2 3 7 5
3 5 4 2 1
2 2 5 4 5
4 4 5 2 3
1 2 4 2 2
3 3 5 2 4
```




```output1
16
NO ESCAPE
-90
27
```



## Note

<p>The figure for the first test case is in the statement. There are only $2$ possible paths to $(n, m)$: </p><ul> <li> Ram travels to $(1, 3)$, takes the ladder to $(3, 3)$, travels to $(3, 2)$, takes the ladder to $(5, 1)$, travels to $(5, 3)$ where he finally escapes via helicopter. The health lost would be $$ \begin{align*} &amp;\mathrel{\phantom{=}} x_1 \cdot |1-3| - h_1 + x_3 \cdot |3-2| - h_3 + x_5 \cdot |1-3| \\ &amp;= 5 \cdot 2 - 4 + 8 \cdot 1 - 6 + 4 \cdot 2 \\ &amp;= 16. \end{align*} $$ </li><li> Ram travels to $(1, 3)$, takes the ladder to $(3, 3)$, travels to $(3, 1)$, takes the ladder to $(5, 2)$, travels to $(5, 3)$ where he finally escapes via helicopter. The health lost would be $$ \begin{align*} &amp;\mathrel{\phantom{=}} x_1 \cdot |1-3| - h_1 + x_3 \cdot |3-1| - h_2 + a_5 \cdot |2-3| \\ &amp;= 5 \cdot 2 - 4 + 8 \cdot 2 - 5 + 4 \cdot 1 \\ &amp;= 21. \end{align*} $$ </li></ul> Therefore, the minimum health lost would be $16$.<p>In the second test case, there is no path to $(n, m)$.</p><p>In the third case case, Ram travels to $(1, 3)$ and takes the only ladder to $(5, 3)$. He loses $5 \cdot 2$ health points and gains $h_1 = 100$ health points. Therefore the total loss is $10-100=-90$ (negative implies he gains health after the path).</p>
