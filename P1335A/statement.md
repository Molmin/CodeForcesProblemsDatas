## Description

<div><p>There are two sisters Alice and Betty. You have $n$ candies. You want to distribute these $n$ candies between two sisters in such a way that:</p><ul> <li> Alice will get $a$ ($a &gt; 0$) candies; </li><li> Betty will get $b$ ($b &gt; 0$) candies; </li><li> each sister will get some <span class="tex-font-style-bf">integer</span> number of candies; </li><li> Alice will get a greater amount of candies than Betty (i.e. $a &gt; b$); </li><li> all the candies will be given to one of two sisters (i.e. $a+b=n$). </li></ul><p>Your task is to calculate the number of ways to distribute exactly $n$ candies between sisters in a way described above. Candies are indistinguishable.</p><p>Formally, find the number of ways to represent $n$ as the sum of $n=a+b$, where $a$ and $b$ are positive integers and $a&gt;b$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of a test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^9$) — the number of candies you have.</p></div><div class="output-specification"><p>For each test case, print the answer — the number of ways to distribute exactly $n$ candies between two sisters in a way described in the problem statement. If there is no way to satisfy all the conditions, print $0$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of a test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^9$) — the number of candies you have.</p>

## Output

<p>For each test case, print the answer — the number of ways to distribute exactly $n$ candies between two sisters in a way described in the problem statement. If there is no way to satisfy all the conditions, print $0$.</p>





```input1
6
7
1
2
3
2000000000
763243547
```




```output1
3
0
0
1
999999999
381621773
```



## Note

<p>For the test case of the example, the $3$ possible ways to distribute candies are:</p><ul> <li> $a=6$, $b=1$; </li><li> $a=5$, $b=2$; </li><li> $a=4$, $b=3$. </li></ul>
