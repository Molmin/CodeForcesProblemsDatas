## Description

<div><p>Not so long ago, Vlad came up with an interesting function:</p><ul><li> $f_a(x)=\left\lfloor\frac{x}{a}\right\rfloor + x \bmod a$, where $\left\lfloor\frac{x}{a}\right\rfloor$ is $\frac{x}{a}$, rounded <span class="tex-font-style-bf">down</span>, $x \bmod a$ — the remainder of the integer division of $x$ by $a$.</li></ul><p>For example, with $a=3$ and $x=11$, the value $f_3(11) = \left\lfloor\frac{11}{3}\right\rfloor + 11 \bmod 3 = 3 + 2 = 5$.</p><p>The number $a$ is fixed and known to Vlad. Help Vlad find the maximum value of $f_a(x)$ if $x$ can take any integer value from $l$ to $r$ inclusive ($l \le x \le r$).</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input test cases.</p><p>This is followed by $t$ lines, each of which contains three integers $l_i$, $r_i$ and $a_i$ ($1 \le l_i \le r_i \le 10^9, 1 \le a_i \le 10^9$)&nbsp;— the left and right boundaries of the segment and the fixed value of $a$.</p></div><div class="output-specification"><p>For each test case, output one number on a separate line&nbsp;— the maximum value of the function on a given segment for a given $a$.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input test cases.</p><p>This is followed by $t$ lines, each of which contains three integers $l_i$, $r_i$ and $a_i$ ($1 \le l_i \le r_i \le 10^9, 1 \le a_i \le 10^9$)&nbsp;— the left and right boundaries of the segment and the fixed value of $a$.</p>

## Output

<p>For each test case, output one number on a separate line&nbsp;— the maximum value of the function on a given segment for a given $a$.</p>





```input1
5
1 4 3
5 8 4
6 10 6
1 1000000000 1000000000
10 12 8
```




```output1
2
4
5
999999999
5
```



## Note

<p>In the first sample:</p><ul> <li> $f_3(1) = \left\lfloor\frac{1}{3}\right\rfloor + 1 \bmod 3 = 0 + 1 = 1$, </li><li> $f_3(2) = \left\lfloor\frac{2}{3}\right\rfloor + 2 \bmod 3 = 0 + 2 = 2$, </li><li> $f_3(3) = \left\lfloor\frac{3}{3}\right\rfloor + 3 \bmod 3 = 1 + 0 = 1$, </li><li> $f_3(4) = \left\lfloor\frac{4}{3}\right\rfloor + 4 \bmod 3 = 1 + 1 = 2$ </li></ul><p>As an answer, obviously, $f_3(2)$ and $f_3(4)$ are suitable.</p>
