## Description

<div><p>There are $n$ cells, numbered $1,2,\dots, n$ from left to right. You have to place a robot at any cell initially. The robot must make <span class="tex-font-style-bf">exactly</span> $k$ moves.</p><p>In one move, the robot must move one cell to the left or right, provided that it doesn't move out of bounds. In other words, if the robot was in the cell $i$, it must move to either the cell $i-1$ or the cell $i+1$, as long as it lies between $1$ and $n$ (endpoints inclusive). The cells, in the order they are visited (including the cell the robot is placed), together make a <span class="tex-font-style-it">good path</span>.</p><p>Each cell $i$ has a value $a_i$ associated with it. Let $c_0, c_1, \dots, c_k$ be the sequence of cells in a <span class="tex-font-style-it">good path</span> in the order they are visited ($c_0$ is the cell robot is initially placed, $c_1$ is the cell where the robot is after its first move, and so on; more formally, $c_i$ is the cell that the robot is at after $i$ moves). Then the value of the path is calculated as $a_{c_0} + a_{c_1} + \dots + a_{c_k}$.</p><p>Your task is to calculate the sum of values over all possible <span class="tex-font-style-it">good paths</span>. Since this number can be very large, output it modulo $10^9 + 7$. Two <span class="tex-font-style-it">good paths</span> are considered different if the starting cell differs or there exists an integer $i \in [1, k]$ such that the current cell of the robot after exactly $i$ moves is different in those paths.</p><p>You must process $q$ updates to $a$ and print the updated sum each time. Each update changes the value of exactly one cell. See the input format and the sample input-output for more details.</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers $n$, $k$ and $q$ ($2 \le n \le 5000$; $1 \le k \le 5000$; $1 \le q \le 2 \cdot 10^5$).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>$q$ lines follow. Each line contains two space-separated integers $i$ and $x$ ($1 \le i \le n$; $1 \le x \le 10^9$) indicating that you must change the value of $a_i$ to $x$.</p></div><div class="output-specification"><p>Print $q$ integers. The $i$-th integer should be the sum of values over all <span class="tex-font-style-it">good paths</span> after the first $i$ updates are performed. Since the answers may be large, print them modulo $10^9 + 7$.</p></div>

## Input

<p>The first line of the input contains three space-separated integers $n$, $k$ and $q$ ($2 \le n \le 5000$; $1 \le k \le 5000$; $1 \le q \le 2 \cdot 10^5$).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>$q$ lines follow. Each line contains two space-separated integers $i$ and $x$ ($1 \le i \le n$; $1 \le x \le 10^9$) indicating that you must change the value of $a_i$ to $x$.</p>

## Output

<p>Print $q$ integers. The $i$-th integer should be the sum of values over all <span class="tex-font-style-it">good paths</span> after the first $i$ updates are performed. Since the answers may be large, print them modulo $10^9 + 7$.</p>





```input1
5 1 5
3 5 1 4 2
1 9
2 4
3 6
4 6
5 2
```




```input2
5 2 5
3 5 1 4 2
1 9
2 4
3 6
4 6
5 2
```




```input3
4 40 6
92 21 82 46
3 56
1 72
4 28
1 97
2 49
2 88
```




```output1
62
58
78
86
86
```




```output2
157
147
207
227
227
```




```output3
239185261
666314041
50729936
516818968
766409450
756910476
```



## Note

<p>In the first example, the <span class="tex-font-style-it">good paths</span> are $(1, 2), (2, 1), (2, 3), (3, 2), (3, 4), (4, 3), (4, 5), (5, 4)$.</p><p>Initially the values of $a$ are $[3, 5, 1, 4, 2]$. After the first update, they become $[9, 5, 1, 4, 2]$. After the second update, they become $[9, 4, 1, 4, 2]$, and so on.</p>
