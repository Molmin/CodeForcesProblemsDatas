## Description

<div><p>Let's define $S(x)$ to be the sum of digits of number $x$ written in decimal system. For example, $S(5) = 5$, $S(10) = 1$, $S(322) = 7$.</p><p>We will call an integer $x$ <span class="tex-font-style-bf">interesting</span> if $S(x + 1) &lt; S(x)$. In each test you will be given one integer $n$. Your task is to calculate the number of integers $x$ such that $1 \le x \le n$ and $x$ is interesting.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) &nbsp;— number of test cases.</p><p>Then $t$ lines follow, the $i$-th line contains one integer $n$ ($1 \le n \le 10^9$) for the $i$-th test case.</p></div><div class="output-specification"><p>Print $t$ integers, the $i$-th should be the answer for the $i$-th test case.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) &nbsp;— number of test cases.</p><p>Then $t$ lines follow, the $i$-th line contains one integer $n$ ($1 \le n \le 10^9$) for the $i$-th test case.</p>

## Output

<p>Print $t$ integers, the $i$-th should be the answer for the $i$-th test case.</p>





```input1
5
1
9
10
34
880055535
```




```output1
0
1
1
3
88005553
```



## Note

<p>The first interesting number is equal to $9$.</p>
