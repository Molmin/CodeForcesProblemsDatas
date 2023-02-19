## Description

<div><p>Fishingprince is playing with an array $[a_1,a_2,\dots,a_n]$. He also has a magic number $m$.</p><p>He can do the following two operations on it:</p><ul> <li> Select $1\le i\le n$ such that $a_i$ is divisible by $m$ (that is, there exists an integer $t$ such that $m \cdot t = a_i$). Replace $a_i$ with <span class="tex-font-style-bf">$m$ copies</span> of $\frac{a_i}{m}$. The order of the other elements doesn't change. For example, when $m=2$ and $a=[2,3]$ and $i=1$, $a$ changes into $[1,1,3]$. </li><li> Select $1\le i\le n-m+1$ such that $a_i=a_{i+1}=\dots=a_{i+m-1}$. Replace these $m$ elements with <span class="tex-font-style-bf">a single</span> $m \cdot a_i$. The order of the other elements doesn't change. For example, when $m=2$ and $a=[3,2,2,3]$ and $i=2$, $a$ changes into $[3,4,3]$. </li></ul><p>Note that the array length might change during the process. The value of $n$ above is defined as the current length of the array (might differ from the $n$ in the input).</p><p>Fishingprince has another array $[b_1,b_2,\dots,b_k]$. Please determine if he can turn $a$ into $b$ using any number (possibly zero) of operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\le n\le 5\cdot 10^4$, $2\le m\le 10^9$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le 10^9$).</p><p>The third line of each test case contains one integer $k$ ($1\le k\le 5\cdot 10^4$).</p><p>The fourth line of each test case contains $k$ integers $b_1,b_2,\ldots,b_k$ ($1\le b_i\le 10^9$).</p><p>It is guaranteed that the sum of $n+k$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print <span class="tex-font-style-tt">Yes</span> if it is possible to turn $a$ into $b$, and <span class="tex-font-style-tt">No</span> otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\le n\le 5\cdot 10^4$, $2\le m\le 10^9$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le 10^9$).</p><p>The third line of each test case contains one integer $k$ ($1\le k\le 5\cdot 10^4$).</p><p>The fourth line of each test case contains $k$ integers $b_1,b_2,\ldots,b_k$ ($1\le b_i\le 10^9$).</p><p>It is guaranteed that the sum of $n+k$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each testcase, print <span class="tex-font-style-tt">Yes</span> if it is possible to turn $a$ into $b$, and <span class="tex-font-style-tt">No</span> otherwise. You can print each letter in any case (upper or lower).</p>





```input1|2,3,4,5,10,11,12,13,18,19,20,21
5
5 2
1 2 2 4 2
4
1 4 4 2
6 2
1 2 2 8 2 2
2
1 16
8 3
3 3 3 3 3 3 3 3
4
6 6 6 6
8 3
3 9 6 3 12 12 36 12
16
9 3 2 2 2 3 4 12 4 12 4 12 4 12 4 4
8 3
3 9 6 3 12 12 36 12
7
12 2 4 3 4 12 56
```




```output1
Yes
Yes
No
Yes
No
```



## Note

<p>In the first test case of the sample, we can do the second operation with $i=2$: $[1,\color{red}{2,2},4,2]\to [1,\color{red}{4},4,2]$.</p><p>In the second testcase of the sample, we can:</p><ul> <li> do the second operation with $i=2$: $[1,\color{red}{2,2},8,2,2]\to [1,\color{red}{4},8,2,2]$. </li><li> do the second operation with $i=4$: $[1,4,8,\color{red}{2,2}]\to [1,4,8,\color{red}{4}]$. </li><li> do the first operation with $i=3$: $[1,4,\color{red}{8},4]\to [1,4,\color{red}{4,4},4]$. </li><li> do the second operation with $i=2$: $[1,\color{red}{4,4},4,4]\to [1,\color{red}{8},4,4]$. </li><li> do the second operation with $i=3$: $[1,8,\color{red}{4,4}]\to [1,8,\color{red}{8}]$. </li><li> do the second operation with $i=2$: $[1,\color{red}{8,8}]\to [1,\color{red}{16}]$.</li></ul>
