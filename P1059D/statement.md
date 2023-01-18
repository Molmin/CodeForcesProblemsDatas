## Description

<div><p>There is a forest that we model as a plane and live $n$ rare animals. Animal number $i$ has its lair in the point $(x_{i}, y_{i})$. In order to protect them, a decision to build a nature reserve has been made.</p><p>The reserve must have a form of a circle containing all lairs. There is also a straight river flowing through the forest. All animals drink from this river, therefore it must have at least one common point with the reserve. On the other hand, ships constantly sail along the river, so the reserve must not have more than one common point with the river.</p><p>For convenience, scientists have made a transformation of coordinates so that the river is defined by $y = 0$. Check whether it is possible to build a reserve, and if possible, find the minimum possible radius of such a reserve.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 10^5$) — the number of animals. </p><p>Each of the next $n$ lines contains two integers $x_{i}$, $y_{i}$ ($-10^7 \le x_{i}, y_{i} \le 10^7$) — the coordinates of the $i$-th animal's lair. It is guaranteed that $y_{i} \neq 0$. No two lairs coincide.</p></div><div class="output-specification"><p>If the reserve cannot be built, print $-1$. Otherwise print the minimum radius. Your answer will be accepted if absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is considered correct if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 10^5$) — the number of animals. </p><p>Each of the next $n$ lines contains two integers $x_{i}$, $y_{i}$ ($-10^7 \le x_{i}, y_{i} \le 10^7$) — the coordinates of the $i$-th animal's lair. It is guaranteed that $y_{i} \neq 0$. No two lairs coincide.</p>

## Output

<p>If the reserve cannot be built, print $-1$. Otherwise print the minimum radius. Your answer will be accepted if absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is considered correct if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$.</p>





```input1
1
0 1

```




```input2
3
0 1
0 2
0 -3

```




```input3
2
0 1
1 1

```




```output1
0.5
```




```output2
-1

```




```output3
0.625
```



## Note

<p>In the first sample it is optimal to build the reserve with the radius equal to $0.5$ and the center in $(0,\ 0.5)$.</p><p>In the second sample it is impossible to build a reserve.</p><p>In the third sample it is optimal to build the reserve with the radius equal to $\frac{5}{8}$ and the center in $(\frac{1}{2},\ \frac{5}{8})$.</p>
