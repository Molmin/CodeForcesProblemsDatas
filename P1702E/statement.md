## Description

<div><p>Polycarp was recently given a set of $n$ (number $n$&nbsp;— even) dominoes. Each domino contains two integers from $1$ to $n$.</p><p>Can he divide all the dominoes into two sets so that all the numbers on the dominoes of each set are different? Each domino must go into exactly one of the two sets.</p><p>For example, if he has $4$ dominoes: $\{1, 4\}$, $\{1, 3\}$, $\{3, 2\}$ and $\{4, 2\}$, then Polycarp will be able to divide them into two sets in the required way. The first set can include the first and third dominoes ($\{1, 4\}$ and $\{3, 2\}$), and the second set&nbsp;— the second and fourth ones ($\{1, 3\}$ and $\{4, 2\}$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single even integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of dominoes.</p><p>The next $n$ lines contain pairs of numbers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$) describing the numbers on the $i$-th domino.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if it is possible to divide $n$ dominoes into two sets so that the numbers on the dominoes of each set are different; </li><li> <span class="tex-font-style-tt">NO</span> if this is not possible. </li></ul><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single even integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of dominoes.</p><p>The next $n$ lines contain pairs of numbers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$) describing the numbers on the $i$-th domino.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if it is possible to divide $n$ dominoes into two sets so that the numbers on the dominoes of each set are different; </li><li> <span class="tex-font-style-tt">NO</span> if this is not possible. </li></ul><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p>





```input1|2,3,4,5,6,14,15,16,20,21,22,23,24,25,26,27,28
6
4
1 2
4 3
2 1
3 4
6
1 2
4 5
1 3
4 6
2 3
5 6
2
1 1
2 2
2
1 2
2 1
8
2 1
1 2
4 3
4 3
5 6
5 7
8 6
7 8
8
1 2
2 1
4 3
5 3
5 4
6 7
8 6
7 8
```




```output1
YES
NO
NO
YES
YES
NO
```



## Note

<p>In the first test case, the dominoes can be divided as follows: </p><ul> <li> First set of dominoes: $[\{1, 2\}, \{4, 3\}]$ </li><li> Second set of dominoes: $[\{2, 1\}, \{3, 4\}]$ </li></ul> In other words, in the first set we take dominoes with numbers $1$ and $2$, and in the second set we take dominoes with numbers $3$ and $4$.<p>In the second test case, there's no way to divide dominoes into $2$ sets, at least one of them will contain repeated number.</p>
