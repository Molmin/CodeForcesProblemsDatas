## Description

<div><p>$n$ towns are arranged in a circle sequentially. The towns are numbered from $1$ to $n$ in clockwise order. In the $i$-th town, there lives a singer with a repertoire of $a_i$ minutes for each $i \in [1, n]$.</p><p>Each singer visited all $n$ towns in clockwise order, starting with the town he lives in, and gave exactly one concert in each town. In addition, in each town, the $i$-th singer got inspired and came up with a song that lasts $a_i$ minutes. The song was added to his repertoire so that he could perform it in the rest of the cities.</p><p>Hence, for the $i$-th singer, the concert in the $i$-th town will last $a_i$ minutes, in the $(i + 1)$-th town the concert will last $2 \cdot a_i$ minutes, ..., in the $((i + k) \bmod n + 1)$-th town the duration of the concert will be $(k + 2) \cdot a_i$, ..., in the town $((i + n - 2) \bmod n + 1)$ — $n \cdot a_i$ minutes.</p><p>You are given an array of $b$ integer numbers, where $b_i$ is the total duration of concerts in the $i$-th town. Reconstruct any correct sequence of <span class="tex-font-style-bf">positive</span> integers $a$ or say that it is impossible.</p></div><div class="input-specification"><p>The first line contains one integer $t$ $(1 \le t \le 10^3$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of two lines. The first line contains a single integer $n$ ($1 \le n \le 4 \cdot 10^4$) — the number of cities. The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^{9}$) — the total duration of concerts in $i$-th city.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the answer as follows:</p><p>If there is no suitable sequence $a$, print <span class="tex-font-style-tt">NO</span>. Otherwise, on the first line print <span class="tex-font-style-tt">YES</span>, on the next line print the sequence $a_1, a_2, \dots, a_n$ of $n$ integers, where $a_i$ ($1 \le a_i \le 10^{9}$) is the initial duration of repertoire of the $i$-th singer. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ $(1 \le t \le 10^3$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of two lines. The first line contains a single integer $n$ ($1 \le n \le 4 \cdot 10^4$) — the number of cities. The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^{9}$) — the total duration of concerts in $i$-th city.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the answer as follows:</p><p>If there is no suitable sequence $a$, print <span class="tex-font-style-tt">NO</span>. Otherwise, on the first line print <span class="tex-font-style-tt">YES</span>, on the next line print the sequence $a_1, a_2, \dots, a_n$ of $n$ integers, where $a_i$ ($1 \le a_i \le 10^{9}$) is the initial duration of repertoire of the $i$-th singer. If there are multiple answers, print any of them.</p>





```input1
4
3
12 16 14
1
1
3
1 2 3
6
81 75 75 93 93 87
```




```output1
YES
3 1 3 
YES
1 
NO
YES
5 5 4 1 4 5
```



## Note

<p>Let's consider the $1$-st test case of the example:</p><ol> <li> the $1$-st singer in the $1$-st city will give a concert for $3$ minutes, in the $2$-nd — for $6$ minutes, in the $3$-rd — for $9$ minutes; </li><li> the $2$-nd singer in the $1$-st city will give a concert for $3$ minutes, in the $2$-nd — for $1$ minute, in the $3$-rd - for $2$ minutes; </li><li> the $3$-rd singer in the $1$-st city will give a concert for $6$ minutes, in the $2$-nd — for $9$ minutes, in the $3$-rd — for $3$ minutes. </li></ol>
