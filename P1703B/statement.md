## Description

<div><p>In an ICPC contest, balloons are distributed as follows: </p><ul> <li> Whenever a team solves a problem, that team gets a balloon. </li><li> The first team to solve a problem gets an additional balloon. </li></ul> A contest has 26 problems, labelled $\textsf{A}$, $\textsf{B}$, $\textsf{C}$, ..., $\textsf{Z}$. You are given the order of solved problems in the contest, denoted as a string $s$, where the $i$-th character indicates that the problem $s_i$ has been solved by some team. No team will solve the same problem twice.<p>Determine the total number of balloons that the teams received. Note that some problems may be solved by none of the teams.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of uppercase English letters, denoting the order of solved problems.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the total number of balloons that the teams received.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of uppercase English letters, denoting the order of solved problems.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the total number of balloons that the teams received.</p>





```input1|2,3,6,7,10,11
6
3
ABA
1
A
3
ORZ
5
BAAAA
4
BKPT
10
CODEFORCES
```




```output1
5
2
6
7
8
17
```



## Note

<p>In the first test case, $5$ balloons are given out: </p><ul> <li> Problem $\textsf{A}$ is solved. That team receives $2$ balloons: one because they solved the problem, an an additional one because they are the first team to solve problem $\textsf{A}$. </li><li> Problem $\textsf{B}$ is solved. That team receives $2$ balloons: one because they solved the problem, an an additional one because they are the first team to solve problem $\textsf{B}$. </li><li> Problem $\textsf{A}$ is solved. That team receives only $1$ balloon, because they solved the problem. Note that they don't get an additional balloon because they are <span class="tex-font-style-bf">not</span> the first team to solve problem $\textsf{A}$. </li></ul> The total number of balloons given out is $2+2+1=5$.<p>In the second test case, there is only one problem solved. The team who solved it receives $2$ balloons: one because they solved the problem, an an additional one because they are the first team to solve problem $\textsf{A}$.</p>
