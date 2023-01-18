## Description

<div><p>You are given two integers $a$ and $b$. You may perform any number of operations on them (possibly zero).</p><p>During each operation you should choose any positive integer $x$ and set $a := a - x$, $b := b - 2x$ or $a := a - 2x$, $b := b - x$. Note that you may choose different values of $x$ in different operations.</p><p>Is it possible to make $a$ and $b$ equal to $0$ simultaneously?</p><p>Your program should answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then the test cases follow, each test case is represented by one line containing two integers $a$ and $b$ for this test case ($0 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>For each test case print the answer to it — <span class="tex-font-style-tt">YES</span> if it is possible to make $a$ and $b$ equal to $0$ simultaneously, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then the test cases follow, each test case is represented by one line containing two integers $a$ and $b$ for this test case ($0 \le a, b \le 10^9$).</p>

## Output

<p>For each test case print the answer to it — <span class="tex-font-style-tt">YES</span> if it is possible to make $a$ and $b$ equal to $0$ simultaneously, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
3
6 9
1 1
1 2
```




```output1
YES
NO
YES
```



## Note

<p>In the first test case of the example two operations can be used to make both $a$ and $b$ equal to zero:</p><ol> <li> choose $x = 4$ and set $a := a - x$, $b := b - 2x$. Then $a = 6 - 4 = 2$, $b = 9 - 8 = 1$; </li><li> choose $x = 1$ and set $a := a - 2x$, $b := b - x$. Then $a = 2 - 2 = 0$, $b = 1 - 1 = 0$. </li></ol>
