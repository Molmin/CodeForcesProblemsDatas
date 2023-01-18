## Description

<div><p>You are given two positive integers $a$ and $b$.</p><p>In one move, you can <span class="tex-font-style-bf">change</span> $a$ in the following way:</p><ul> <li> Choose any positive <span class="tex-font-style-bf">odd</span> integer $x$ ($x &gt; 0$) and replace $a$ with $a+x$; </li><li> choose any positive <span class="tex-font-style-bf">even</span> integer $y$ ($y &gt; 0$) and replace $a$ with $a-y$. </li></ul><p>You can perform as many such operations as you want. You can choose the same numbers $x$ and $y$ in different moves.</p><p>Your task is to find the minimum number of moves required to obtain $b$ from $a$. It is guaranteed that you can always obtain $b$ from $a$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Then $t$ test cases follow. Each test case is given as two space-separated integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the answer — the minimum number of moves required to obtain $b$ from $a$ if you can perform any number of moves described in the problem statement. It is guaranteed that you can always obtain $b$ from $a$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Then $t$ test cases follow. Each test case is given as two space-separated integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p>

## Output

<p>For each test case, print the answer — the minimum number of moves required to obtain $b$ from $a$ if you can perform any number of moves described in the problem statement. It is guaranteed that you can always obtain $b$ from $a$.</p>





```input1
5
2 3
10 10
2 4
7 4
9 3
```




```output1
1
0
2
2
1
```



## Note

<p>In the first test case, you can just add $1$.</p><p>In the second test case, you don't need to do anything.</p><p>In the third test case, you can add $1$ two times.</p><p>In the fourth test case, you can subtract $4$ and add $1$.</p><p>In the fifth test case, you can just subtract $6$.</p>
