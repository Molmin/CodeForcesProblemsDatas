## Description

<div><p>You were dreaming that you are traveling to a planet named Planetforces on your personal spaceship. Unfortunately, its piloting system was corrupted and now you need to fix it in order to reach Planetforces.</p><center> <img class="tex-graphics" src="file://kOARwn45.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Space can be represented as the $XY$ plane. You are starting at point $(0, 0)$, and Planetforces is located in point $(p_x, p_y)$.</p><p>The piloting system of your spaceship follows its list of orders which can be represented as a string $s$. The system reads $s$ from left to right. Suppose you are at point $(x, y)$ and current order is $s_i$: </p><ul> <li> if $s_i = \text{U}$, you move to $(x, y + 1)$; </li><li> if $s_i = \text{D}$, you move to $(x, y - 1)$; </li><li> if $s_i = \text{R}$, you move to $(x + 1, y)$; </li><li> if $s_i = \text{L}$, you move to $(x - 1, y)$. </li></ul><p>Since string $s$ could be corrupted, there is a possibility that you won't reach Planetforces in the end. Fortunately, <span class="tex-font-style-bf">you can delete some orders from $s$ but you can't change their positions</span>.</p><p>Can you delete several orders (possibly, zero) from $s$ in such a way, that you'll reach Planetforces after the system processes all orders?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. The first line in each test case contains two integers $p_x$ and $p_y$ ($-10^5 \le p_x, p_y \le 10^5$; $(p_x, p_y) \neq (0, 0)$)&nbsp;— the coordinates of Planetforces $(p_x, p_y)$.</p><p>The second line contains the string $s$ ($1 \le |s| \le 10^5$: $|s|$ is the length of string $s$)&nbsp;— the list of orders.</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if you can delete several orders (possibly, zero) from $s$ in such a way, that you'll reach Planetforces. Otherwise, print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. The first line in each test case contains two integers $p_x$ and $p_y$ ($-10^5 \le p_x, p_y \le 10^5$; $(p_x, p_y) \neq (0, 0)$)&nbsp;— the coordinates of Planetforces $(p_x, p_y)$.</p><p>The second line contains the string $s$ ($1 \le |s| \le 10^5$: $|s|$ is the length of string $s$)&nbsp;— the list of orders.</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if you can delete several orders (possibly, zero) from $s$ in such a way, that you'll reach Planetforces. Otherwise, print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p>





```input1
6
10 5
RRRRRRRRRRUUUUU
1 1
UDDDRLLL
-3 -5
LDLDLDDDR
1 2
LLLLUU
3 -2
RDULRLLDR
-1 6
RUDURUUUUR
```




```output1
YES
YES
YES
NO
YES
NO
```



## Note

<p>In the first case, you don't need to modify $s$, since the given $s$ will bring you to Planetforces.</p><p>In the second case, you can delete orders $s_2$, $s_3$, $s_4$, $s_6$, $s_7$ and $s_8$, so $s$ becomes equal to "<span class="tex-font-style-tt">UR</span>".</p><p>In the third test case, you have to delete order $s_9$, otherwise, you won't finish in the position of Planetforces.</p>
