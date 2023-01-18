## Description

<div><p>Let $f_{x} = c^{2x-6} \cdot f_{x-1} \cdot f_{x-2} \cdot f_{x-3}$ for $x \ge 4$.</p><p>You have given integers $n$, $f_{1}$, $f_{2}$, $f_{3}$, and $c$. Find $f_{n} \bmod (10^{9}+7)$.</p></div><div class="input-specification"><p>The only line contains five integers $n$, $f_{1}$, $f_{2}$, $f_{3}$, and $c$ ($4 \le n \le 10^{18}$, $1 \le f_{1}$, $f_{2}$, $f_{3}$, $c \le 10^{9}$).</p></div><div class="output-specification"><p>Print $f_{n} \bmod (10^{9} + 7)$.</p></div>

## Input

<p>The only line contains five integers $n$, $f_{1}$, $f_{2}$, $f_{3}$, and $c$ ($4 \le n \le 10^{18}$, $1 \le f_{1}$, $f_{2}$, $f_{3}$, $c \le 10^{9}$).</p>

## Output

<p>Print $f_{n} \bmod (10^{9} + 7)$.</p>





```input1
5 1 2 5 3
```




```input2
17 97 41 37 11
```




```output1
72900
```




```output2
317451037
```



## Note

<p>In the first example, $f_{4} = 90$, $f_{5} = 72900$.</p><p>In the second example, $f_{17} \approx 2.28 \times 10^{29587}$.</p>
