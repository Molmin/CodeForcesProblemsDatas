## Description

<div><p>Consider the set of all nonnegative integers: ${0, 1, 2, \dots}$. Given two integers $a$ and $b$ ($1 \le a, b \le 10^4$). We paint all the numbers in increasing number first we paint $0$, then we paint $1$, then $2$ and so on.</p><p>Each number is painted white or black. We paint a number $i$ according to the following rules: </p><ul>  <li> if $i = 0$, it is colored white;  </li><li> if $i \ge a$ and $i - a$ is colored white, $i$ is also colored white;  </li><li> if $i \ge b$ and $i - b$ is colored white, $i$ is also colored white;  </li><li> if $i$ is still not colored white, it is colored black. </li></ul><p>In this way, each nonnegative integer gets one of two colors.</p><p>For example, if $a=3$, $b=5$, then the colors of the numbers (in the order from $0$) are: white ($0$), black ($1$), black ($2$), white ($3$), black ($4$), white ($5$), white ($6$), black ($7$), white ($8$), white ($9$), ...</p><p>Note that: </p><ul>  <li> It is possible that there are infinitely many nonnegative integers colored black. For example, if $a = 10$ and $b = 10$, then only $0, 10, 20, 30$ and any other nonnegative integers that end in $0$ when written in base 10 are white. The other integers are colored black.  </li><li> It is also possible that there are only finitely many nonnegative integers colored black. For example, when $a = 1$ and $b = 10$, then there is no nonnegative integer colored black at all. </li></ul><p>Your task is to determine whether or not the number of nonnegative integers colored <span class="tex-font-style-bf">black</span> is infinite.</p><p>If there are infinitely many nonnegative integers colored black, simply print a line containing "<span class="tex-font-style-tt">Infinite</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">Finite</span>" (without the quotes).</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases in the input. Then $t$ lines follow, each line contains two space-separated integers $a$ and $b$ ($1 \le a, b \le 10^4$).</p></div><div class="output-specification"><p>For each test case, print one line containing either "<span class="tex-font-style-tt">Infinite</span>" or "<span class="tex-font-style-tt">Finite</span>" (without the quotes). Output is case-insensitive (i.e. "<span class="tex-font-style-tt">infinite</span>", "<span class="tex-font-style-tt">inFiNite</span>" or "<span class="tex-font-style-tt">finiTE</span>" are all valid answers).</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases in the input. Then $t$ lines follow, each line contains two space-separated integers $a$ and $b$ ($1 \le a, b \le 10^4$).</p>

## Output

<p>For each test case, print one line containing either "<span class="tex-font-style-tt">Infinite</span>" or "<span class="tex-font-style-tt">Finite</span>" (without the quotes). Output is case-insensitive (i.e. "<span class="tex-font-style-tt">infinite</span>", "<span class="tex-font-style-tt">inFiNite</span>" or "<span class="tex-font-style-tt">finiTE</span>" are all valid answers).</p>





```input1
4
10 10
1 10
6 9
7 3
```




```output1
Infinite
Finite
Infinite
Finite
```


