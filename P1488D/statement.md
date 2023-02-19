## Description

<div><p>Polycarp has decided to do a problemsolving marathon. He wants to solve $s$ problems in $n$ days. Let $a_i$ be the number of problems he solves during the $i$-th day. He wants to find a distribution of problems into days such that: </p><ul> <li> $a_i$ is an integer value for all $i$ from $1$ to $n$; </li><li> $a_i \ge 1$ for all $i$ from $1$ to $n$; </li><li> $a_{i + 1} \ge a_i$ for all $i$ from $1$ to $n-1$; </li><li> $a_{i + 1} \le 2 \cdot a_i$ for all $i$ from $1$ to $n-1$; </li><li> $a_n$ is maximized. </li></ul><p>Note that $a_1$ can be arbitrarily large.</p><p>What is the largest value of $a_n$ Polycarp can obtain?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains two integers $n$ and $s$ ($1 \le n \le s \le 10^{18}$)&nbsp;— the number of days and the number of problems Polycarp wants to solve.</p><p>It's guaranteed that the distribution always exists within the given constraints.</p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the maximum value of $a_n$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains two integers $n$ and $s$ ($1 \le n \le s \le 10^{18}$)&nbsp;— the number of days and the number of problems Polycarp wants to solve.</p><p>It's guaranteed that the distribution always exists within the given constraints.</p>

## Output

<p>For each testcase print a single integer&nbsp;— the maximum value of $a_n$.</p>





```input1
3
1 15
3 9
2 6
```




```output1
15
4
4
```



## Note

<p>In the first testcase there is only one distribution: $[15]$.</p><p>In the second testcase the distribution that maximizes $a_n$ is: $[2, 3, 4]$.</p><p>In the third testcase the distribution that maximizes $a_n$ is: $[2, 4]$. $[3, 3]$ is a valid distribution but $a_n=3$ which is smaller than $4$. $[1, 5]$ is not a valid distribution because $5 &gt; 2 \cdot 1$.</p>
