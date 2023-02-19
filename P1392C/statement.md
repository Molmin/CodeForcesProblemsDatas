## Description

<div><p>Omkar is building a waterslide in his water park, and he needs your help to ensure that he does it as efficiently as possible.</p><p>Omkar currently has $n$ supports arranged in a line, the $i$-th of which has height $a_i$. Omkar wants to build his waterslide from the right to the left, so his supports must be nondecreasing in height in order to support the waterslide. In $1$ operation, Omkar can do the following: take any <span class="tex-font-style-bf">contiguous subsegment</span> of supports which is <span class="tex-font-style-bf">nondecreasing by heights</span> and add $1$ to each of their heights. </p><p>Help Omkar find the minimum number of operations he needs to perform to make his supports able to support his waterslide!</p><p>An array $b$ is a subsegment of an array $c$ if $b$ can be obtained from $c$ by deletion of several (possibly zero or all) elements from the beginning and several (possibly zero or all) elements from the end.</p><p>An array $b_1, b_2, \dots, b_n$ is called nondecreasing if $b_i\le b_{i+1}$ for every $i$ from $1$ to $n-1$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of supports Omkar has.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},...,a_{n}$ $(0 \leq a_{i} \leq 10^9)$&nbsp;— the heights of the supports.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum number of operations Omkar needs to perform to make his supports able to support his waterslide.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of supports Omkar has.</p><p>The second line of each test case contains $n$ integers $a_{1},a_{2},...,a_{n}$ $(0 \leq a_{i} \leq 10^9)$&nbsp;— the heights of the supports.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum number of operations Omkar needs to perform to make his supports able to support his waterslide.</p>





```input1
3
4
5 3 2 5
5
1 2 3 5 3
3
1 1 1
```




```output1
3
2
0
```



## Note

<p>The subarray with which Omkar performs the operation is bolded.</p><p>In the first test case:</p><ul><li><p>First operation:</p><p>$[5, 3, \textbf{2}, 5] \to [5, 3, \textbf{3}, 5]$</p></li><li><p>Second operation:</p><p>$[5, \textbf{3}, \textbf{3}, 5] \to [5, \textbf{4}, \textbf{4}, 5]$</p></li><li><p>Third operation:</p><p>$[5, \textbf{4}, \textbf{4}, 5] \to [5, \textbf{5}, \textbf{5}, 5]$</p></li></ul><p>In the third test case, the array is already nondecreasing, so Omkar does $0$ operations.</p>
