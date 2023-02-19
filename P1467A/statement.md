## Description

<div><p>There are $n$ digital panels placed in a straight line. Each panel can show any digit from $0$ to $9$. Initially, all panels show $0$.</p><p>Every second, the digit shown by each panel increases by $1$. In other words, at the end of every second, a panel that showed $9$ would now show $0$, a panel that showed $0$ would now show $1$, a panel that showed $1$ would now show $2$, and so on.</p><p>When a panel is paused, the digit displayed on the panel does not change in the subsequent seconds.</p><p>You must pause exactly one of these panels, at any second you wish. Then, the panels adjacent to it get paused one second later, the panels adjacent to those get paused $2$ seconds later, and so on. In other words, if you pause panel $x$, panel $y$ (for all valid $y$) would be paused exactly $|x−y|$ seconds later.</p><p>For example, suppose there are $4$ panels, and the $3$-rd panel is paused when the digit $9$ is on it.</p><ul> <li> The panel $1$ pauses $2$ seconds later, so it has the digit $1$; </li><li> the panel $2$ pauses $1$ second later, so it has the digit $0$; </li><li> the panel $4$ pauses $1$ second later, so it has the digit $0$. </li></ul><p>The resulting $4$-digit number is $1090$. <span class="tex-font-style-bf">Note that this example is not optimal for $n = 4$</span>.</p><p>Once all panels have been paused, you write the digits displayed on them from left to right, to form an $n$ digit number (it can consist of leading zeros). What is the largest possible number you can get? Initially, all panels show $0$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Each test case consists of a single line containing a single integer $n$ ($1 \le n \le 2\cdot10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print the largest number you can achieve, if you pause one panel optimally.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Each test case consists of a single line containing a single integer $n$ ($1 \le n \le 2\cdot10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print the largest number you can achieve, if you pause one panel optimally.</p>





```input1
2
1
2
```




```output1
9
98
```



## Note

<p>In the first test case, it is optimal to pause the first panel when the number $9$ is displayed on it.</p><p>In the second test case, it is optimal to pause the second panel when the number $8$ is displayed on it.</p>
