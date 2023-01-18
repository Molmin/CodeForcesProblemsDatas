## Description

<div><p>You're at the last mission in one very old and very popular strategy game Dune II: Battle For Arrakis. The map of the mission can be represented as a rectangular matrix of size $n \times m$. Initially, there are $a_{i, j}$ units of your army in the cell $(i, j)$.</p><p>You want to prepare for the final battle, so you want to move all your army into <span class="tex-font-style-bf">exactly one cell</span> of the map (i.e. $nm-1$ cells should contain $0$ units of the army and the remaining cell should contain the entire army).</p><p>To do this, you can do some (possibly, zero) number of moves. During one move, you can select <span class="tex-font-style-bf">exactly one unit</span> from some cell and move it to one of the adjacent <span class="tex-font-style-bf">by side</span> cells. I.e. from the cell $(i, j)$ you can move the unit to cells:</p><ul> <li> $(i - 1, j)$; </li><li> $(i, j - 1)$; </li><li> $(i + 1, j)$; </li><li> $(i, j + 1)$. </li></ul><p>Of course, you want to move all your army into <span class="tex-font-style-bf">exactly one cell</span> as fast as possible. So, you want to know the <span class="tex-font-style-bf">minimum</span> number of moves you need to do that.</p><p>And, of course, life goes on, so the situation on the map changes. There are $q$ updates, the $i$-th update is denoted by three integers $x, y, z$. This update affects the army in the cell $(x, y)$: after this update, the number of units in the cell $(x, y)$ becomes $z$ (i.e. you replace $a_{x, y}$ with $z$).</p><p>Also, you want to determine, for each $i$, the <span class="tex-font-style-bf">minimum</span> number of moves needed to move your entire army into <span class="tex-font-style-bf">exactly one cell</span> with the first $i$ updates applied to the initial map. In other words, the map after the $i$-th update equals the <span class="tex-font-style-bf">initial</span> map with the first $i$ updates applied to it.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, m$ and $q$ ($1 \le n, m \le 1000; 1 \le q \le 5000$)&nbsp;— the size of the matrix and the number of updates correspondingly.</p><p>The next $n$ lines contain $m$ integers each, where the $j$-th integer in the $i$-th line is $a_{i, j}$ ($1 \le a_{i, j} \le 10^9$)&nbsp;— the number of units in the cell $(i, j)$.</p><p>The next $q$ lines contain three integers each, where the $i$-th line contains three integers $x_i, y_i$ and $z_i$ ($1 \le x_i \le n; 1 \le y_i \le m; 1 \le z_i \le 10^9$)&nbsp;— the cell in which the number of units updates and the new number of units in this cell correspondingly.</p></div><div class="output-specification"><p>Print $q+1$ integers $r_0, r_1, r_2, \dots, r_n$, where $r_0$ is the <span class="tex-font-style-bf">minimum</span> number of moves you need to move all your army into <span class="tex-font-style-bf">exactly one cell</span>, and $r_i$ for all $i$ from $1$ to $q$ is the <span class="tex-font-style-bf">minimum</span> number of moves you need to move all your army into <span class="tex-font-style-bf">exactly one cell</span> after the first $i$ updates.</p></div>

## Input

<p>The first line of the input contains three integers $n, m$ and $q$ ($1 \le n, m \le 1000; 1 \le q \le 5000$)&nbsp;— the size of the matrix and the number of updates correspondingly.</p><p>The next $n$ lines contain $m$ integers each, where the $j$-th integer in the $i$-th line is $a_{i, j}$ ($1 \le a_{i, j} \le 10^9$)&nbsp;— the number of units in the cell $(i, j)$.</p><p>The next $q$ lines contain three integers each, where the $i$-th line contains three integers $x_i, y_i$ and $z_i$ ($1 \le x_i \le n; 1 \le y_i \le m; 1 \le z_i \le 10^9$)&nbsp;— the cell in which the number of units updates and the new number of units in this cell correspondingly.</p>

## Output

<p>Print $q+1$ integers $r_0, r_1, r_2, \dots, r_n$, where $r_0$ is the <span class="tex-font-style-bf">minimum</span> number of moves you need to move all your army into <span class="tex-font-style-bf">exactly one cell</span>, and $r_i$ for all $i$ from $1$ to $q$ is the <span class="tex-font-style-bf">minimum</span> number of moves you need to move all your army into <span class="tex-font-style-bf">exactly one cell</span> after the first $i$ updates.</p>





```input1
3 3 1
1 2 3
2 1 2
1 1 2
2 3 100
```




```input2
4 4 3
2 5 6 3
4 8 10 5
2 6 7 1
8 4 2 1
1 1 8
2 3 4
4 4 5
```




```output1
21 22
```




```output2
123 135 129 145
```


