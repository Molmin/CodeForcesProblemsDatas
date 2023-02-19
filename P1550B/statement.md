## Description

<div><p>You are given a string $s$ of length $n$ consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>You perform the following operation until the string becomes empty: choose some <span class="tex-font-style-bf">consecutive</span> substring of <span class="tex-font-style-bf">equal</span> characters, erase it from the string and glue the remaining two parts together (any of them can be empty) in the same order. For example, if you erase the substring <span class="tex-font-style-tt">111</span> from the string <span class="tex-font-style-tt">1<span class="tex-font-style-bf">111</span>10</span>, you will get the string <span class="tex-font-style-tt">110</span>. When you delete a substring of length $l$, you get $a \cdot l + b$ points.</p><p>Your task is to calculate the maximum number of points that you can score in total, if you have to make the given string empty.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n$, $a$ and $b$ ($1 \le n \le 100; -100 \le a, b \le 100$)&nbsp;— the length of the string $s$ and the parameters $a$ and $b$.</p><p>The second line contains the string $s$. The string $s$ consists only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the maximum number of points that you can score.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains three integers $n$, $a$ and $b$ ($1 \le n \le 100; -100 \le a, b \le 100$)&nbsp;— the length of the string $s$ and the parameters $a$ and $b$.</p><p>The second line contains the string $s$. The string $s$ consists only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the maximum number of points that you can score.</p>





```input1
3
3 2 0
000
5 -2 5
11001
6 1 -4
100111
```




```output1
6
15
-2
```



## Note

<p>In the first example, it is enough to delete the entire string, then we will get $2 \cdot 3 + 0 = 6$ points.</p><p>In the second example, if we delete characters one by one, then for each deleted character we will get $(-2) \cdot 1 + 5 = 3$ points, i. e. $15$ points in total.</p><p>In the third example, we can delete the substring <span class="tex-font-style-tt">00</span> from the string <span class="tex-font-style-tt">1<span class="tex-font-style-bf">00</span>111</span>, we get $1 \cdot 2 + (-4) = -2$ points, and the string will be equal to <span class="tex-font-style-tt">1111</span>, removing it entirely we get $1 \cdot 4 + (-4) = 0$ points. In total, we got $-2$ points for $2$ operations.</p>
