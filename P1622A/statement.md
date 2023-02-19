## Description

<div><p>There are three sticks with integer lengths $l_1, l_2$ and $l_3$.</p><p>You are asked to break exactly one of them into two pieces in such a way that: </p><ul> <li> both pieces have positive (strictly greater than $0$) <span class="tex-font-style-bf">integer</span> length; </li><li> the total length of the pieces is equal to the original length of the stick; </li><li> it's possible to construct a rectangle from the resulting four sticks such that each stick is used as exactly one of its sides. </li></ul><p>A square is also considered a rectangle.</p><p>Determine if it's possible to do that.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains three integers $l_1, l_2, l_3$ ($1 \le l_i \le 10^8$)&nbsp;— the lengths of the sticks.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if it's possible to break one of the sticks into two pieces with positive integer length in such a way that it's possible to construct a rectangle from the resulting four sticks. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains three integers $l_1, l_2, l_3$ ($1 \le l_i \le 10^8$)&nbsp;— the lengths of the sticks.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if it's possible to break one of the sticks into two pieces with positive integer length in such a way that it's possible to construct a rectangle from the resulting four sticks. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as a positive answer).</p>





```input1
4
6 1 5
2 5 2
2 4 2
5 5 4
```




```output1
YES
NO
YES
YES
```



## Note

<p>In the first testcase, the first stick can be broken into parts of length $1$ and $5$. We can construct a rectangle with opposite sides of length $1$ and $5$.</p><p>In the second testcase, breaking the stick of length $2$ can only result in sticks of lengths $1, 1, 2, 5$, which can't be made into a rectangle. Breaking the stick of length $5$ can produce results $2, 3$ or $1, 4$ but neither of them can't be put into a rectangle.</p><p>In the third testcase, the second stick can be broken into parts of length $2$ and $2$. The resulting rectangle has opposite sides $2$ and $2$ (which is a square).</p><p>In the fourth testcase, the third stick can be broken into parts of length $2$ and $2$. The resulting rectangle has opposite sides $2$ and $5$.</p>
