## Description

<div><p>Igor had a sequence $d_1, d_2, \dots, d_n$ of integers. When Igor entered the classroom there was an integer $x$ written on the blackboard.</p><p>Igor generated sequence $p$ using the following algorithm: </p><ol> <li> initially, $p = [x]$; </li><li> for each $1 \leq i \leq n$ he did the following operation $|d_i|$ times: <ul> <li> if $d_i \geq 0$, then he looked at the last element of $p$ (let it be $y$) and appended $y + 1$ to the end of $p$; </li><li> if $d_i &lt; 0$, then he looked at the last element of $p$ (let it be $y$) and appended $y - 1$ to the end of $p$. </li></ul> </li></ol><p>For example, if $x = 3$, and $d = [1, -1, 2]$, $p$ will be equal $[3, 4, 3, 4, 5]$.</p><p>Igor decided to calculate the length of the longest increasing subsequence of $p$ and the number of them.</p><p>A sequence $a$ is a subsequence of a sequence $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p><p>A sequence $a$ is an increasing sequence if each element of $a$ (except the first one) is strictly greater than the previous element.</p><p>For $p = [3, 4, 3, 4, 5]$, the length of longest increasing subsequence is $3$ and there are $3$ of them: $[\underline{3}, \underline{4}, 3, 4, \underline{5}]$, $[\underline{3}, 4, 3, \underline{4}, \underline{5}]$, $[3, 4, \underline{3}, \underline{4}, \underline{5}]$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the sequence $d$.</p><p>The second line contains a single integer $x$ ($-10^9 \leq x \leq 10^9$)&nbsp;— the integer on the blackboard.</p><p>The third line contains $n$ integers $d_1, d_2, \ldots, d_n$ ($-10^9 \leq d_i \leq 10^9$).</p></div><div class="output-specification"><p>Print two integers: </p><ul> <li> the first integer should be equal to the length of the longest increasing subsequence of $p$; </li><li> the second should be equal to the number of them modulo $998244353$. </li></ul><p>You should print <span class="tex-font-style-it">only the second number</span> modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the sequence $d$.</p><p>The second line contains a single integer $x$ ($-10^9 \leq x \leq 10^9$)&nbsp;— the integer on the blackboard.</p><p>The third line contains $n$ integers $d_1, d_2, \ldots, d_n$ ($-10^9 \leq d_i \leq 10^9$).</p>

## Output

<p>Print two integers: </p><ul> <li> the first integer should be equal to the length of the longest increasing subsequence of $p$; </li><li> the second should be equal to the number of them modulo $998244353$. </li></ul><p>You should print <span class="tex-font-style-it">only the second number</span> modulo $998244353$.</p>





```input1
3
3
1 -1 2
```




```input2
3
100
5 -3 6
```




```input3
3
1
999999999 0 1000000000
```




```input4
5
34
1337 -146 42 -69 228
```




```output1
3 3
```




```output2
9 7
```




```output3
2000000000 1
```




```output4
1393 3876
```



## Note

<p>The first test case was explained in the statement.</p><p>In the second test case $p = [100, 101, 102, 103, 104, 105, 104, 103, 102, 103, 104, 105, 106, 107, 108]$.</p><p>In the third test case $p = [1, 2, \ldots, 2000000000]$.</p>
