## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$, consisting of $n$ <span class="tex-font-style-bf">positive</span> integers. </p><p>Initially you are standing at index $1$ and have a score equal to $a_1$. You can perform two kinds of moves: </p><ol> <li> move right&nbsp;— go from your current index $x$ to $x+1$ and add $a_{x+1}$ to your score. This move can only be performed if $x&lt;n$. </li><li> move left&nbsp;— go from your current index $x$ to $x-1$ and add $a_{x-1}$ to your score. This move can only be performed if $x&gt;1$. <span class="tex-font-style-bf">Also, you can't perform two or more moves to the left in a row.</span> </li></ol><p>You want to perform <span class="tex-font-style-bf">exactly</span> $k$ moves. Also, there should be no more than $z$ moves to the left among them.</p><p>What is the maximum score you can achieve?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n, k$ and $z$ ($2 \le n \le 10^5$, $1 \le k \le n - 1$, $0 \le z \le min(5, k)$)&nbsp;— the number of elements in the array, the total number of moves you should perform and the maximum number of moves to the left you can perform.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^4$)&nbsp;— the given array.</p><p>The sum of $n$ over all testcases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ integers&nbsp;— for each testcase output the maximum score you can achieve if you make exactly $k$ moves in total, no more than $z$ of them are to the left and there are no two or more moves to the left in a row.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n, k$ and $z$ ($2 \le n \le 10^5$, $1 \le k \le n - 1$, $0 \le z \le min(5, k)$)&nbsp;— the number of elements in the array, the total number of moves you should perform and the maximum number of moves to the left you can perform.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^4$)&nbsp;— the given array.</p><p>The sum of $n$ over all testcases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>Print $t$ integers&nbsp;— for each testcase output the maximum score you can achieve if you make exactly $k$ moves in total, no more than $z$ of them are to the left and there are no two or more moves to the left in a row.</p>





```input1
4
5 4 0
1 5 4 3 2
5 4 1
1 5 4 3 2
5 4 4
10 20 30 40 50
10 7 3
4 6 8 2 9 9 7 4 10 9
```




```output1
15
19
150
56
```



## Note

<p>In the first testcase you are not allowed to move left at all. So you make four moves to the right and obtain the score $a_1 + a_2 + a_3 + a_4 + a_5$.</p><p>In the second example you can move one time to the left. So we can follow these moves: right, right, left, right. The score will be $a_1 + a_2 + a_3 + a_2 + a_3$.</p><p>In the third example you can move four times to the left but it's not optimal anyway, you can just move four times to the right and obtain the score $a_1 + a_2 + a_3 + a_4 + a_5$.</p>
