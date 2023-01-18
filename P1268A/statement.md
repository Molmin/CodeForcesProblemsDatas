## Description

<div><p>You are given an integer $x$ of $n$ digits $a_1, a_2, \ldots, a_n$, which make up its decimal notation in order from left to right.</p><p>Also, you are given a positive integer $k &lt; n$.</p><p>Let's call integer $b_1, b_2, \ldots, b_m$ <span class="tex-font-style-bf">beautiful</span> if $b_i = b_{i+k}$ for each $i$, such that $1 \leq i \leq m - k$.</p><p>You need to find the smallest <span class="tex-font-style-bf">beautiful</span> integer $y$, such that $y \geq x$. </p></div><div class="input-specification"><p>The first line of input contains two integers $n, k$ ($2 \leq n \leq 200\,000, 1 \leq k &lt; n$): the number of digits in $x$ and $k$.</p><p>The next line of input contains $n$ digits $a_1, a_2, \ldots, a_n$ ($a_1 \neq 0$, $0 \leq a_i \leq 9$): digits of $x$.</p></div><div class="output-specification"><p>In the first line print one integer $m$: the number of digits in $y$.</p><p>In the next line print $m$ digits $b_1, b_2, \ldots, b_m$ ($b_1 \neq 0$, $0 \leq b_i \leq 9$): digits of $y$.</p></div>

## Input

<p>The first line of input contains two integers $n, k$ ($2 \leq n \leq 200\,000, 1 \leq k &lt; n$): the number of digits in $x$ and $k$.</p><p>The next line of input contains $n$ digits $a_1, a_2, \ldots, a_n$ ($a_1 \neq 0$, $0 \leq a_i \leq 9$): digits of $x$.</p>

## Output

<p>In the first line print one integer $m$: the number of digits in $y$.</p><p>In the next line print $m$ digits $b_1, b_2, \ldots, b_m$ ($b_1 \neq 0$, $0 \leq b_i \leq 9$): digits of $y$.</p>





```input1
3 2
353
```




```input2
4 2
1234
```




```output1
3
353
```




```output2
4
1313
```


