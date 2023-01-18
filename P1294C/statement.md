## Description

<div><p>You are given one integer number $n$. Find three <span class="tex-font-style-bf">distinct integers</span> $a, b, c$ such that $2 \le a, b, c$ and $a \cdot b \cdot c = n$ or say that it is impossible to do it.</p><p>If there are several answers, you can print any.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The next $n$ lines describe test cases. The $i$-th test case is given on a new line as one integer $n$ ($2 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the answer on it. Print "<span class="tex-font-style-tt">NO</span>" if it is impossible to represent $n$ as $a \cdot b \cdot c$ for some <span class="tex-font-style-bf">distinct integers</span> $a, b, c$ such that $2 \le a, b, c$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> possible such representation.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The next $n$ lines describe test cases. The $i$-th test case is given on a new line as one integer $n$ ($2 \le n \le 10^9$).</p>

## Output

<p>For each test case, print the answer on it. Print "<span class="tex-font-style-tt">NO</span>" if it is impossible to represent $n$ as $a \cdot b \cdot c$ for some <span class="tex-font-style-bf">distinct integers</span> $a, b, c$ such that $2 \le a, b, c$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> possible such representation.</p>





```input1
5
64
32
97
2
12345
```




```output1
YES
2 4 8 
NO
NO
NO
YES
3 5 823
```


