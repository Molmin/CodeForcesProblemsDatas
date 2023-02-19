## Description

<div><p>You have a string $s$ consisting of digits from $0$ to $9$ inclusive. You can perform the following operation any (possibly zero) number of times: </p><ul> <li> You can choose a position $i$ and delete a digit $d$ on the $i$-th position. Then insert the digit $\min{(d + 1, 9)}$ on any position (at the beginning, at the end or in between any two adjacent digits). </li></ul><p>What is the lexicographically smallest string you can get by performing these operations?</p><p>A string $a$ is lexicographically smaller than a string $b$ of the same length if and only if the following holds: </p><ul> <li> in the first position where $a$ and $b$ differ, the string $a$ has a smaller digit than the corresponding digit in $b$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of a single line that contains one string $s$ ($1 \le |s| \le 2 \cdot 10^5$) — the string consisting of digits. Please note that $s$ is just a string consisting of digits, so leading zeros are allowed.</p><p>It is guaranteed that the sum of lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print a single string — the minimum string that is possible to obtain.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of a single line that contains one string $s$ ($1 \le |s| \le 2 \cdot 10^5$) — the string consisting of digits. Please note that $s$ is just a string consisting of digits, so leading zeros are allowed.</p><p>It is guaranteed that the sum of lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print a single string — the minimum string that is possible to obtain.</p>





```input1|2,4
4
04829
9
01
314752277691991
```




```output1
02599
9
01
111334567888999
```



## Note

<p>In the first test case: </p><ul> <li> Delete $8$ and insert $9$ at the end of the notation. The resulting notation is $04299$. </li><li> Delete $4$ and insert $5$ in the $3$-rd position of the notation. The resulting notation is $02599$. </li></ul><p>Nothing needs to be done in the second and third test cases.</p>
