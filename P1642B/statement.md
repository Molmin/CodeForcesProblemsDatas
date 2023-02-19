## Description

<div><p>Sam is a kindergartener, and there are $n$ children in his group. He decided to create a team with some of his children to play "brawl:go 2".</p><p>Sam has $n$ power-ups, the $i$-th has type $a_i$. A child's strength is equal to the number of <span class="tex-font-style-bf">different</span> types among power-ups he has.</p><p>For a team of size $k$, Sam will distribute all $n$ power-ups to $k$ children in such a way that each of the $k$ children receives at least one power-up, and each power-up is given to someone.</p><p>For each integer $k$ from $1$ to $n$, find the <span class="tex-font-style-bf">minimum</span> sum of strengths of a team of $k$ children Sam can get.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$). </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — types of Sam's power-ups.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For every test case print $n$ integers.</p><p>The $k$-th integer should be equal to the minimum sum of strengths of children in the team of size $k$ that Sam can get.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$). </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — types of Sam's power-ups.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For every test case print $n$ integers.</p><p>The $k$-th integer should be equal to the minimum sum of strengths of children in the team of size $k$ that Sam can get.</p>





```input1
2
3
1 1 2
6
5 1 2 2 2 4
```




```output1
2 2 3 
4 4 4 4 5 6
```



## Note

<p>One of the ways to give power-ups to minimise the sum of strengths in the first test case: </p><ul> <li> $k = 1: \{1, 1, 2\}$   </li><li> $k = 2: \{1, 1\}, \{2\}$   </li><li> $k = 3: \{1\}, \{1\}, \{2\}$   </li></ul><p>One of the ways to give power-ups to minimise the sum of strengths in the second test case: </p><ul> <li> $k = 1: \{1, 2, 2, 2, 4, 5\}$   </li><li> $k = 2: \{2, 2, 2, 4, 5\}, \{1\}$   </li><li> $k = 3: \{2, 2, 2, 5\}, \{1\}, \{4\}$   </li><li> $k = 4: \{2, 2, 2\}, \{1\}, \{4\}, \{5\}$   </li><li> $k = 5: \{2, 2\}, \{1\}, \{2\}, \{4\}, \{5\}$   </li><li> $k = 6: \{1\}, \{2\}, \{2\}, \{2\}, \{4\}, \{5\}$   </li></ul>
