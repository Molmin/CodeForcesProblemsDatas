## Description

<div><p>To become the king of Codeforces, Kuroni has to solve the following problem.</p><p>He is given $n$ numbers $a_1, a_2, \dots, a_n$. Help Kuroni to calculate $\prod_{1\le i&lt;j\le n} |a_i - a_j|$. As result can be very big, output it modulo $m$.</p><p>If you are not familiar with short notation, $\prod_{1\le i&lt;j\le n} |a_i - a_j|$ is equal to $|a_1 - a_2|\cdot|a_1 - a_3|\cdot$ $\dots$ $\cdot|a_1 - a_n|\cdot|a_2 - a_3|\cdot|a_2 - a_4|\cdot$ $\dots$ $\cdot|a_2 - a_n| \cdot$ $\dots$ $\cdot |a_{n-1} - a_n|$. In other words, this is the product of $|a_i - a_j|$ for all $1\le i &lt; j \le n$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($2\le n \le 2\cdot 10^5$, $1\le m \le 1000$)&nbsp;— number of numbers and modulo.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Output the single number&nbsp;— $\prod_{1\le i&lt;j\le n} |a_i - a_j| \bmod m$.</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($2\le n \le 2\cdot 10^5$, $1\le m \le 1000$)&nbsp;— number of numbers and modulo.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p>

## Output

<p>Output the single number&nbsp;— $\prod_{1\le i&lt;j\le n} |a_i - a_j| \bmod m$.</p>





```input1
2 10
8 5
```




```input2
3 12
1 4 5
```




```input3
3 7
1 4 9
```




```output1
3
```




```output2
0
```




```output3
1
```



## Note

<p>In the first sample, $|8 - 5| = 3 \equiv 3 \bmod 10$.</p><p>In the second sample, $|1 - 4|\cdot|1 - 5|\cdot|4 - 5| = 3\cdot 4 \cdot 1 = 12 \equiv 0 \bmod 12$.</p><p>In the third sample, $|1 - 4|\cdot|1 - 9|\cdot|4 - 9| = 3 \cdot 8 \cdot 5 = 120 \equiv 1 \bmod 7$.</p>
