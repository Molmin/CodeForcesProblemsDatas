## Description

<div><p><span class="tex-font-style-bf">Note that the memory limit in this problem is lower than in others.</span></p><p>You have a vertical strip with $n$ cells, numbered consecutively from $1$ to $n$ from top to bottom.</p><p>You also have a token that is initially placed in cell $n$. You will move the token up until it arrives at cell $1$.</p><p>Let the token be in cell $x &gt; 1$ at some moment. One shift of the token can have either of the following kinds: </p><ul> <li> Subtraction: you choose an integer $y$ between $1$ and $x-1$, inclusive, and move the token from cell $x$ to cell $x - y$. </li><li> Floored division: you choose an integer $z$ between $2$ and $x$, inclusive, and move the token from cell $x$ to cell $\lfloor \frac{x}{z} \rfloor$ ($x$ divided by $z$ rounded down). </li></ul><p>Find the number of ways to move the token from cell $n$ to cell $1$ using one or more shifts, and print it modulo $m$. Note that if there are several ways to move the token from one cell to another in one shift, all these ways are considered <span class="tex-font-style-bf">distinct</span> (check example explanation for a better understanding).</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($2 \le n \le 4 \cdot 10^6$; $10^8 &lt; m &lt; 10^9$; $m$ is a prime number)&nbsp;— the length of the strip and the modulo.</p></div><div class="output-specification"><p>Print the number of ways to move the token from cell $n$ to cell $1$, modulo $m$.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($2 \le n \le 4 \cdot 10^6$; $10^8 &lt; m &lt; 10^9$; $m$ is a prime number)&nbsp;— the length of the strip and the modulo.</p>

## Output

<p>Print the number of ways to move the token from cell $n$ to cell $1$, modulo $m$.</p>





```input1
3 998244353
```




```input2
5 998244353
```




```input3
42 998244353
```




```input4
787788 100000007
```




```output1
5
```




```output2
25
```




```output3
793019428
```




```output4
94810539
```



## Note

<p>In the first test, there are three ways to move the token from cell $3$ to cell $1$ in one shift: using subtraction of $y = 2$, or using division by $z = 2$ or $z = 3$.</p><p>There are also two ways to move the token from cell $3$ to cell $1$ via cell $2$: first subtract $y = 1$, and then either subtract $y = 1$ again or divide by $z = 2$.</p><p>Therefore, there are five ways in total.</p>
