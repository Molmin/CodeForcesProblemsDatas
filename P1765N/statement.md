## Description

<div><p>You are given a positive integer $x$.</p><p>You can apply the following operation to the number: remove one occurrence of any digit in such a way that the resulting number <span class="tex-font-style-bf">does not contain any leading zeroes</span> and <span class="tex-font-style-bf">is still a positive integer</span>. For example, $10142$ can be converted to $1142$, $1042$, $1012$ or $1014$ (note that $0142$ is not a valid outcome); $10$ can be converted to $1$ (but not to $0$ since it is not positive).</p><p>Your task is to find the minimum positive integer that you can obtain from $x$ if you can apply the aforementioned operation exactly $k$ times.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x &lt; 10^{500000}$).</p><p>The second line contains a single integer $k$ ($0 \le k &lt; |x|$), where $|x|$ is the length of the number $x$.</p><p>The sum of $|x|$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum positive number that you can obtain from $x$ if you can apply the operation exactly $k$ times.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x &lt; 10^{500000}$).</p><p>The second line contains a single integer $k$ ($0 \le k &lt; |x|$), where $|x|$ is the length of the number $x$.</p><p>The sum of $|x|$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum positive number that you can obtain from $x$ if you can apply the operation exactly $k$ times.</p>





```input1|2,3,6,7,10,11
5
10000
4
1337
0
987654321
6
66837494128
5
7808652
3
```




```output1
1
1337
321
344128
7052
```


