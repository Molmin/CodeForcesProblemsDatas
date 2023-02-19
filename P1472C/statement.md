## Description

<div><p>Polycarp found under the Christmas tree an array $a$ of $n$ elements and instructions for playing with it: </p><ul> <li> At first, choose index $i$ ($1 \leq i \leq n$)&nbsp;— starting position in the array. Put the chip at the index $i$ (on the value $a_i$). </li><li> While $i \leq n$, add $a_i$ to your score and move the chip $a_i$ positions to the right (i.e. replace $i$ with $i + a_i$). </li><li> If $i &gt; n$, then Polycarp ends the game. </li></ul><p>For example, if $n = 5$ and $a = [7, 3, 1, 2, 3]$, then the following game options are possible: </p><ul> <li> Polycarp chooses $i = 1$. Game process: $i = 1 \overset{+7}{\longrightarrow} 8$. The score of the game is: $a_1 = 7$. </li><li> Polycarp chooses $i = 2$. Game process: $i = 2 \overset{+3}{\longrightarrow} 5 \overset{+3}{\longrightarrow} 8$. The score of the game is: $a_2 + a_5 = 6$. </li><li> Polycarp chooses $i = 3$. Game process: $i = 3 \overset{+1}{\longrightarrow} 4 \overset{+2}{\longrightarrow} 6$. The score of the game is: $a_3 + a_4 = 3$. </li><li> Polycarp chooses $i = 4$. Game process: $i = 4 \overset{+2}{\longrightarrow} 6$. The score of the game is: $a_4 = 2$. </li><li> Polycarp chooses $i = 5$. Game process: $i = 5 \overset{+3}{\longrightarrow} 8$. The score of the game is: $a_5 = 3$. </li></ul><p>Help Polycarp to find out the maximum score he can get if he chooses the starting index in an optimal way.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output on a separate line one number&nbsp;— the maximum score that Polycarp can get by playing the game on the corresponding array according to the instruction from the statement. Note that Polycarp chooses any starting position from $1$ to $n$ in such a way as to maximize his result.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output on a separate line one number&nbsp;— the maximum score that Polycarp can get by playing the game on the corresponding array according to the instruction from the statement. Note that Polycarp chooses any starting position from $1$ to $n$ in such a way as to maximize his result.</p>





```input1
4
5
7 3 1 2 3
3
2 1 4
6
2 1000 2 3 995 1
5
1 1 1 1 1
```




```output1
7
6
1000
5
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case, the maximum score can be achieved by choosing $i = 1$.</p><p>In the third test case, the maximum score can be achieved by choosing $i = 2$.</p><p>In the fourth test case, the maximum score can be achieved by choosing $i = 1$.</p>
