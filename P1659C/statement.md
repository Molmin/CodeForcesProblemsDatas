## Description

<div><p><span class="tex-font-style-it">You are an ambitious king who wants to be the Emperor of The Reals. But to do that, you must first become Emperor of The Integers.</span></p><p>Consider a number axis. The capital of your empire is initially at $0$. There are $n$ unconquered kingdoms at positions $0&lt;x_1&lt;x_2&lt;\ldots&lt;x_n$. You want to conquer all other kingdoms.</p><p>There are two actions available to you: </p><ul> <li> You can change the location of your capital (let its current position be $c_1$) to any other <span class="tex-font-style-bf">conquered</span> kingdom (let its position be $c_2$) at a cost of $a\cdot |c_1-c_2|$. </li><li> From the current capital (let its current position be $c_1$) you can conquer an unconquered kingdom (let its position be $c_2$) at a cost of $b\cdot |c_1-c_2|$. You <span class="tex-font-style-bf">cannot</span> conquer a kingdom if there is an unconquered kingdom between the target and your capital. </li></ul><p>Note that you <span class="tex-font-style-bf">cannot</span> place the capital at a point without a kingdom. In other words, at any point, your capital can only be at $0$ or one of $x_1,x_2,\ldots,x_n$. Also note that conquering a kingdom does not change the position of your capital.</p><p>Find the minimum total cost to conquer all kingdoms. Your capital can be anywhere at the end.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of each test case follows.</p><p>The first line of each test case contains $3$ integers $n$, $a$, and $b$ ($1 \leq n \leq 2 \cdot 10^5$; $1 \leq a,b \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \leq x_1 &lt; x_2 &lt; \ldots &lt; x_n \leq 10^8$).</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the minimum cost to conquer all kingdoms.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of each test case follows.</p><p>The first line of each test case contains $3$ integers $n$, $a$, and $b$ ($1 \leq n \leq 2 \cdot 10^5$; $1 \leq a,b \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \leq x_1 &lt; x_2 &lt; \ldots &lt; x_n \leq 10^8$).</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the minimum cost to conquer all kingdoms.</p>





```input1
4
5 2 7
3 5 12 13 21
5 6 3
1 5 6 21 30
2 9 3
10 15
11 27182 31415
16 18 33 98 874 989 4848 20458 34365 38117 72030
```




```output1
173
171
75
3298918744
```



## Note

<p>Here is an optimal sequence of moves for the second test case:</p><ol> <li> Conquer the kingdom at position $1$ with cost $3\cdot(1-0)=3$. </li><li> Move the capital to the kingdom at position $1$ with cost $6\cdot(1-0)=6$. </li><li> Conquer the kingdom at position $5$ with cost $3\cdot(5-1)=12$. </li><li> Move the capital to the kingdom at position $5$ with cost $6\cdot(5-1)=24$. </li><li> Conquer the kingdom at position $6$ with cost $3\cdot(6-5)=3$. </li><li> Conquer the kingdom at position $21$ with cost $3\cdot(21-5)=48$. </li><li> Conquer the kingdom at position $30$ with cost $3\cdot(30-5)=75$. </li></ol><p>The total cost is $3+6+12+24+3+48+75=171$. You cannot get a lower cost than this.</p>
