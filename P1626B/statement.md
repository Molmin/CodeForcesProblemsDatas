## Description

<div><p>You are given a decimal representation of an integer $x$ without leading zeros.</p><p>You have to perform the following reduction on it <span class="tex-font-style-bf">exactly once</span>: take two neighboring digits in $x$ and replace them with their sum without leading zeros (if the sum is $0$, it's represented as a single $0$).</p><p>For example, if $x = 10057$, the possible reductions are: </p><ul> <li> choose the first and the second digits $1$ and $0$, replace them with $1+0=1$; the result is $1057$; </li><li> choose the second and the third digits $0$ and $0$, replace them with $0+0=0$; the result is also $1057$; </li><li> choose the third and the fourth digits $0$ and $5$, replace them with $0+5=5$; the result is still $1057$; </li><li> choose the fourth and the fifth digits $5$ and $7$, replace them with $5+7=12$; the result is $10012$. </li></ul><p>What's the largest number that can be obtained?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single integer $x$ ($10 \le x &lt; 10^{200000}$). $x$ doesn't contain leading zeros.</p><p>The total length of the decimal representations of $x$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the largest number that can be obtained after the reduction is applied exactly once. The number should not contain leading zeros.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Each testcase consists of a single integer $x$ ($10 \le x &lt; 10^{200000}$). $x$ doesn't contain leading zeros.</p><p>The total length of the decimal representations of $x$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the largest number that can be obtained after the reduction is applied exactly once. The number should not contain leading zeros.</p>





```input1
2
10057
90
```




```output1
10012
9
```



## Note

<p>The first testcase of the example is already explained in the statement.</p><p>In the second testcase, there is only one possible reduction: the first and the second digits.</p>
