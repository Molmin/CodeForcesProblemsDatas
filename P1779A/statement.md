## Description

<div><p>Thalia is a Legendary Grandmaster in chess. She has $n$ trophies in a line numbered from $1$ to $n$ (from left to right) and a lamp standing next to each of them (the lamps are numbered as the trophies).</p><p>A lamp can be directed either to the left or to the right, and it illuminates all trophies in that direction (but not the one it is next to). More formally, Thalia has a string $s$ consisting only of characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>' which represents the lamps' current directions. The lamp $i$ illuminates:</p><ul> <li> trophies $1,2,\ldots, i-1$ if $s_i$ is '<span class="tex-font-style-tt">L</span>'; </li><li> trophies $i+1,i+2,\ldots, n$ if $s_i$ is '<span class="tex-font-style-tt">R</span>'. </li></ul><p>She can perform the following operation <span class="tex-font-style-bf">at most</span> once:</p><ul> <li> Choose an index $i$ ($1 \leq i &lt; n$); </li><li> Swap the lamps $i$ and $i+1$ (without changing their directions). That is, swap $s_i$ with $s_{i+1}$. </li></ul><p>Thalia asked you to illuminate all her trophies (make each trophy illuminated by at least one lamp), or to tell her that it is impossible to do so. If it is possible, you can choose to perform an operation or to do nothing. Notice that lamps <span class="tex-font-style-bf">cannot</span> change direction, it is only allowed to swap adjacent ones.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($2 \leq n \leq 100\,000$) &nbsp;— the number of trophies.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting only of characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>' &nbsp;— the $i$-th character describes the direction of the $i$-th lamp.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100\,000$.</p></div><div class="output-specification"><p>For each test case print $-1$ if it is impossible to illuminate all trophies by performing one operation (or doing nothing). Otherwise, print $0$ if you choose not to perform the operation (i.e., the trophies are illuminated by the initial positioning of the lamps), or an index $i$ ($1 \leq i &lt; n$) if you choose to swap lamps $i$ and $i+1$.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($2 \leq n \leq 100\,000$) &nbsp;— the number of trophies.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting only of characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>' &nbsp;— the $i$-th character describes the direction of the $i$-th lamp.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100\,000$.</p>

## Output

<p>For each test case print $-1$ if it is impossible to illuminate all trophies by performing one operation (or doing nothing). Otherwise, print $0$ if you choose not to perform the operation (i.e., the trophies are illuminated by the initial positioning of the lamps), or an index $i$ ($1 \leq i &lt; n$) if you choose to swap lamps $i$ and $i+1$.</p><p>If there are multiple answers, print any.</p>





```input1
6
2
LL
2
LR
2
RL
2
RR
7
LLRLLLR
7
RRLRRRL
```




```output1
-1
1
0
-1
3
6
```



## Note

<p>In the first example, it is possible to swap lamps $1$ and $2$, or do nothing. In any case, the string "<span class="tex-font-style-tt">LL</span>" is obtained. Not all trophies are illuminated since trophy $2$ is not illuminated by any lamp &nbsp;— lamp $1$ illuminates nothing and lamp $2$ illuminates only the trophy $1$.</p><p>In the second example, it is necessary to swap lamps $1$ and $2$. The string becomes "<span class="tex-font-style-tt">RL</span>". Trophy $1$ is illuminated by lamp $2$ and trophy $2$ is illuminated by lamp $1$, hence it is possible to illuminate all trophies.</p><p>In the third example, all trophies are initially illuminated &nbsp;— hence, not performing any operation is a valid solution.</p><p>In the last two examples performing swaps is not necessary as all trophies are illuminated initially. But, the presented solutions are also valid.</p>
