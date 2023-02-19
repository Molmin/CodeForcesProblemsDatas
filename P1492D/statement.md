## Description

<div><p>You are given three integers $a$, $b$, $k$.</p><p>Find two <span class="tex-font-style-it">binary</span> integers $x$ and $y$ ($x \ge y$) such that </p><ol> <li> both $x$ and $y$ consist of $a$ zeroes and $b$ ones; </li><li> $x - y$ (also written in binary form) has exactly $k$ ones. </li></ol> You are <span class="tex-font-style-bf">not allowed to use leading zeros for $x$ and $y$</span>. </div><div class="input-specification"><p>The only line contains three integers $a$, $b$, and $k$ ($0 \leq a$; $1 \leq b$; $0 \leq k \leq a + b \leq 2 \cdot 10^5$)&nbsp;— the number of zeroes, ones, and the number of ones in the result.</p></div><div class="output-specification"><p>If it's possible to find two suitable integers, print "<span class="tex-font-style-tt">Yes</span>" followed by $x$ and $y$ in base-2.</p><p>Otherwise print "<span class="tex-font-style-tt">No</span>".</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The only line contains three integers $a$, $b$, and $k$ ($0 \leq a$; $1 \leq b$; $0 \leq k \leq a + b \leq 2 \cdot 10^5$)&nbsp;— the number of zeroes, ones, and the number of ones in the result.</p>

## Output

<p>If it's possible to find two suitable integers, print "<span class="tex-font-style-tt">Yes</span>" followed by $x$ and $y$ in base-2.</p><p>Otherwise print "<span class="tex-font-style-tt">No</span>".</p><p>If there are multiple possible answers, print any of them.</p>





```input1
4 2 3
```




```input2
3 2 1
```




```input3
3 2 5
```




```output1
Yes
101000
100001
```




```output2
Yes
10100
10010
```




```output3
No
```



## Note

<p>In the first example, $x = 101000_2 = 2^5 + 2^3 = 40_{10}$, $y = 100001_2 = 2^5 + 2^0 = 33_{10}$, $40_{10} - 33_{10} = 7_{10} = 2^2 + 2^1 + 2^0 = 111_{2}$. Hence $x-y$ has $3$ ones in base-2.</p><p>In the second example, $x = 10100_2 = 2^4 + 2^2 = 20_{10}$, $y = 10010_2 = 2^4 + 2^1 = 18$, $x - y = 20 - 18 = 2_{10} = 10_{2}$. This is precisely one 1.</p><p>In the third example, one may show, that it's impossible to find an answer.</p>
