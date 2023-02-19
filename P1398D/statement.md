## Description

<div><p>You are given three multisets of pairs of colored sticks: </p><ul> <li> $R$ pairs of red sticks, the first pair has length $r_1$, the second pair has length $r_2$, $\dots$, the $R$-th pair has length $r_R$; </li><li> $G$ pairs of green sticks, the first pair has length $g_1$, the second pair has length $g_2$, $\dots$, the $G$-th pair has length $g_G$; </li><li> $B$ pairs of blue sticks, the first pair has length $b_1$, the second pair has length $b_2$, $\dots$, the $B$-th pair has length $b_B$; </li></ul><p>You are constructing rectangles from these pairs of sticks with the following process: </p><ol> <li> take a pair of sticks of one color; </li><li> take a pair of sticks of another color different from the first one; </li><li> add the area of the resulting rectangle to the total area. </li></ol><p>Thus, you get such rectangles that their opposite sides are the same color and their adjacent sides are not the same color.</p><p>Each pair of sticks can be used at most once, some pairs can be left unused. You are not allowed to split a pair into independent sticks.</p><p>What is the maximum area you can achieve?</p></div><div class="input-specification"><p>The first line contains three integers $R$, $G$, $B$ ($1 \le R, G, B \le 200$)&nbsp;— the number of pairs of red sticks, the number of pairs of green sticks and the number of pairs of blue sticks.</p><p>The second line contains $R$ integers $r_1, r_2, \dots, r_R$ ($1 \le r_i \le 2000$)&nbsp;— the lengths of sticks in each pair of red sticks.</p><p>The third line contains $G$ integers $g_1, g_2, \dots, g_G$ ($1 \le g_i \le 2000$)&nbsp;— the lengths of sticks in each pair of green sticks.</p><p>The fourth line contains $B$ integers $b_1, b_2, \dots, b_B$ ($1 \le b_i \le 2000$)&nbsp;— the lengths of sticks in each pair of blue sticks.</p></div><div class="output-specification"><p>Print the maximum possible total area of the constructed rectangles.</p></div>

## Input

<p>The first line contains three integers $R$, $G$, $B$ ($1 \le R, G, B \le 200$)&nbsp;— the number of pairs of red sticks, the number of pairs of green sticks and the number of pairs of blue sticks.</p><p>The second line contains $R$ integers $r_1, r_2, \dots, r_R$ ($1 \le r_i \le 2000$)&nbsp;— the lengths of sticks in each pair of red sticks.</p><p>The third line contains $G$ integers $g_1, g_2, \dots, g_G$ ($1 \le g_i \le 2000$)&nbsp;— the lengths of sticks in each pair of green sticks.</p><p>The fourth line contains $B$ integers $b_1, b_2, \dots, b_B$ ($1 \le b_i \le 2000$)&nbsp;— the lengths of sticks in each pair of blue sticks.</p>

## Output

<p>Print the maximum possible total area of the constructed rectangles.</p>





```input1
1 1 1
3
5
4
```




```input2
2 1 3
9 5
1
2 8 5
```




```input3
10 1 1
11 7 20 15 19 14 2 4 13 14
8
11
```




```output1
20
```




```output2
99
```




```output3
372
```



## Note

<p>In the first example you can construct one of these rectangles: red and green with sides $3$ and $5$, red and blue with sides $3$ and $4$ and green and blue with sides $5$ and $4$. The best area of them is $4 \times 5 = 20$.</p><p>In the second example the best rectangles are: red/blue $9 \times 8$, red/blue $5 \times 5$, green/blue $2 \times 1$. So the total area is $72 + 25 + 2 = 99$.</p><p>In the third example the best rectangles are: red/green $19 \times 8$ and red/blue $20 \times 11$. The total area is $152 + 220 = 372$. Note that you can't construct more rectangles because you are not allowed to have both pairs taken to be the same color.</p>
