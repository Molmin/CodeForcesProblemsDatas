## Description

<div><p>Inflation has occurred in Berlandia, so the store needs to change the price of goods.</p><p>The current price of good $n$ is given. It is allowed to increase the price of the good by $k$ times, with $1 \le k \le m$, k is an integer. Output the roundest possible new price of the good. That is, the one that has the maximum number of zeros at the end.</p><p>For example, the number <span class="tex-font-style-tt">481000</span> is more round than the number <span class="tex-font-style-tt">1000010</span> (three zeros at the end of <span class="tex-font-style-tt">481000</span> and only one at the end of <span class="tex-font-style-tt">1000010</span>).</p><p>If there are several possible variants, output the one in which the new price is maximal.</p><p>If it is impossible to get a rounder price, output $n \cdot m$ (that is, the maximum possible price).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>Each test case consists of one line.</p><p>This line contains two integers: $n$ and $m$ ($1 \le n, m \le 10^9$). Where $n$ is the old price of the good, and the number $m$ means that you can increase the price $n$ no more than $m$ times.</p></div><div class="output-specification"><p>For each test case, output on a separate line the roundest integer of the form $n \cdot k$ ($1 \le k \le m$, $k$&nbsp;— an integer).</p><p>If there are several possible variants, output the one in which the new price (value $n \cdot k$) is maximal.</p><p>If it is impossible to get a more rounded price, output $n \cdot m$ (that is, the maximum possible price).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>Each test case consists of one line.</p><p>This line contains two integers: $n$ and $m$ ($1 \le n, m \le 10^9$). Where $n$ is the old price of the good, and the number $m$ means that you can increase the price $n$ no more than $m$ times.</p>

## Output

<p>For each test case, output on a separate line the roundest integer of the form $n \cdot k$ ($1 \le k \le m$, $k$&nbsp;— an integer).</p><p>If there are several possible variants, output the one in which the new price (value $n \cdot k$) is maximal.</p><p>If it is impossible to get a more rounded price, output $n \cdot m$ (that is, the maximum possible price).</p>





```input1|2,4,6,8,10
10
6 11
5 43
13 5
4 16
10050 12345
2 6
4 30
25 10
2 81
1 7
```




```output1
60
200
65
60
120600000
10
100
200
100
7
```



## Note

<p>In the first case $n = 6$, $m = 11$. We cannot get a number with two zeros or more at the end, because we need to increase the price $50$ times, but $50 &gt; m = 11$. The maximum price multiple of $10$ would be $6 \cdot 10 = 60$.</p><p>In the second case $n = 5$, $m = 43$. The maximum price multiple of $100$ would be $5 \cdot 40 = 200$.</p><p>In the third case, $n = 13$, $m = 5$. All possible new prices will not end in $0$, then you should output $n \cdot m = 65$.</p><p>In the fourth case, you should increase the price $15$ times.</p><p>In the fifth case, increase the price $12000$ times.</p>
