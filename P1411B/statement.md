## Description

<div><p>We call a positive integer number <span class="tex-font-style-it">fair</span> if it is divisible by each of its nonzero digits. For example, $102$ is fair (because it is divisible by $1$ and $2$), but $282$ is not, because it isn't divisible by $8$. Given a positive integer $n$. Find the minimum integer $x$, such that $n \leq x$ and $x$ is fair.</p></div><div class="input-specification"><p>The first line contains number of test cases $t$ ($1 \leq t \leq 10^3$). Each of the next $t$ lines contains an integer $n$ ($1 \leq n \leq 10^{18}$).</p></div><div class="output-specification"><p>For each of $t$ test cases print a single integer&nbsp;— the least <span class="tex-font-style-it">fair</span> number, which is not less than $n$.</p></div>

## Input

<p>The first line contains number of test cases $t$ ($1 \leq t \leq 10^3$). Each of the next $t$ lines contains an integer $n$ ($1 \leq n \leq 10^{18}$).</p>

## Output

<p>For each of $t$ test cases print a single integer&nbsp;— the least <span class="tex-font-style-it">fair</span> number, which is not less than $n$.</p>





```input1
4
1
282
1234567890
1000000000000000000
```




```output1
1
288
1234568040
1000000000000000000
```



## Note

<p>Explanations for some test cases: </p><ul> <li> In the first test case number $1$ is fair itself. </li><li> In the second test case number $288$ is fair (it's divisible by both $2$ and $8$). None of the numbers from $[282, 287]$ is fair, because, for example, none of them is divisible by $8$. </li></ul>
