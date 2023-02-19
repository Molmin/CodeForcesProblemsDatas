## Description

<div><p>Vasya decided to go to the grocery store. He found in his wallet $a$ coins of $1$ burle and $b$ coins of $2$ burles. He does not yet know the total cost of all goods, so help him find out $s$ ($s &gt; 0$): the <span class="tex-font-style-bf">minimum</span> positive integer amount of money he <span class="tex-font-style-bf">cannot</span> pay without change or pay at all using only his coins.</p><p>For example, if $a=1$ and $b=1$ (he has one $1$-burle coin and one $2$-burle coin), then:</p><ul> <li> he can pay $1$ burle without change, paying with one $1$-burle coin, </li><li> he can pay $2$ burle without change, paying with one $2$-burle coin, </li><li> he can pay $3$ burle without change by paying with one $1$-burle coin and one $2$-burle coin, </li><li> he cannot pay $4$ burle without change (moreover, he cannot pay this amount at all). </li></ul><p>So for $a=1$ and $b=1$ the answer is $s=4$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The description of each test case consists of one line containing two integers $a_i$ and $b_i$ ($0 \le a_i, b_i \le 10^8$)&nbsp;— the number of $1$-burle coins and $2$-burles coins Vasya has respectively.</p></div><div class="output-specification"><p>For each test case, on a separate line print one integer $s$ ($s &gt; 0$): the minimum positive integer amount of money that Vasya cannot pay without change or pay at all.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The description of each test case consists of one line containing two integers $a_i$ and $b_i$ ($0 \le a_i, b_i \le 10^8$)&nbsp;— the number of $1$-burle coins and $2$-burles coins Vasya has respectively.</p>

## Output

<p>For each test case, on a separate line print one integer $s$ ($s &gt; 0$): the minimum positive integer amount of money that Vasya cannot pay without change or pay at all.</p>





```input1
5
1 1
4 0
0 2
0 0
2314 2374
```




```output1
4
5
1
1
7063
```



## Note

<ul> <li> The first test case of the example is clarified into the main part of the statement. </li><li> In the second test case, Vasya has only $1$ burle coins, and he can collect either any amount from $1$ to $4$, but $5$ can't. </li><li> In the second test case, Vasya has only $2$ burle coins, and he cannot pay $1$ burle without change. </li><li> In the fourth test case you don't have any coins, and he can't even pay $1$ burle. </li></ul>
