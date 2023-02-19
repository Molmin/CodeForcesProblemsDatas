## Description

<div><p>Nezzar has a binary string $s$ of length $n$ that he wants to share with his best friend, Nanako. Nanako will spend $q$ days inspecting the binary string. At the same time, Nezzar wants to change the string $s$ into string $f$ during these $q$ days, because it looks better.</p><p>It is known that Nanako loves consistency so much. On the $i$-th day, Nanako will inspect a segment of string $s$ from position $l_i$ to position $r_i$ inclusive. If the segment contains both characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>', Nanako becomes unhappy and throws away the string.</p><p>After this inspection, at the $i$-th night, Nezzar can secretly change <span class="tex-font-style-bf">strictly less</span> than half of the characters in the segment from $l_i$ to $r_i$ inclusive, otherwise the change will be too obvious.</p><p>Now Nezzar wonders, if it is possible to avoid Nanako being unhappy and at the same time have the string become equal to the string $f$ at the end of these $q$ days and nights.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of test cases.</p><p>The first line of each test case contains two integers $n,q$ ($1 \le n \le 2 \cdot 10^5$, $0 \le q \le 2 \cdot 10^5$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>The third line of each test case contains a binary string $f$ of length $n$.</p><p>Then $q$ lines follow, $i$-th of them contains two integers $l_i,r_i$ ($1 \le l_i \le r_i \le n$) &nbsp;— bounds of the segment, that Nanako will inspect on the $i$-th day.</p><p>It is guaranteed that the sum of $n$ for all test cases doesn't exceed $2 \cdot 10^5$, and the sum of $q$ for all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" on the single line if it is possible to avoid Nanako being unhappy and have the string $f$ at the end of $q$ days and nights. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of test cases.</p><p>The first line of each test case contains two integers $n,q$ ($1 \le n \le 2 \cdot 10^5$, $0 \le q \le 2 \cdot 10^5$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>The third line of each test case contains a binary string $f$ of length $n$.</p><p>Then $q$ lines follow, $i$-th of them contains two integers $l_i,r_i$ ($1 \le l_i \le r_i \le n$) &nbsp;— bounds of the segment, that Nanako will inspect on the $i$-th day.</p><p>It is guaranteed that the sum of $n$ for all test cases doesn't exceed $2 \cdot 10^5$, and the sum of $q$ for all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" on the single line if it is possible to avoid Nanako being unhappy and have the string $f$ at the end of $q$ days and nights. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
5 2
00000
00111
1 5
1 3
2 1
00
01
1 2
10 6
1111111111
0110001110
1 10
5 9
7 10
1 7
3 5
6 10
5 2
10000
11000
2 5
1 3
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first test case, $\underline{00000} \rightarrow \underline{000}11 \rightarrow 00111$ is one of the possible sequences of string changes.</p><p>In the second test case, it can be shown that it is impossible to have the string $f$ at the end.</p>
