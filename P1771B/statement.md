## Description

<div><p>Hossam makes a big party, and he will invite his friends to the party.</p><p>He has $n$ friends numbered from $1$ to $n$. They will be arranged in a queue as follows: $1, 2, 3, \ldots, n$.</p><p>Hossam has a list of $m$ pairs of his friends that don't know each other. Any pair not present in this list are friends.</p><p>A subsegment of the queue starting from the friend $a$ and ending at the friend $b$ is $[a, a + 1, a + 2, \ldots, b]$. A subsegment of the queue is called <span class="tex-font-style-it">good</span> when all pairs of that segment are friends.</p><p>Hossam wants to know how many pairs $(a, b)$ there are ($1 \le a \le b \le n$), such that the subsegment starting from the friend $a$ and ending at the friend $b$ is good.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$), the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integer numbers $n$ and $m$ ($2 \le n \le 10^5$, $0 \le m \le 10^5$) representing the number of friends and the number of pairs, respectively.</p><p>The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i\le n$, $x_i \neq y_i$) representing a pair of Hossam's friends that don't know each other.</p><p>Note that pairs can be repeated.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$, and the sum of $m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print an integer — the number of good subsegments.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$), the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integer numbers $n$ and $m$ ($2 \le n \le 10^5$, $0 \le m \le 10^5$) representing the number of friends and the number of pairs, respectively.</p><p>The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i\le n$, $x_i \neq y_i$) representing a pair of Hossam's friends that don't know each other.</p><p>Note that pairs can be repeated.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$, and the sum of $m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print an integer — the number of good subsegments.</p>





```input1|2,3,4
2
3 2
1 3
2 3
4 2
1 2
2 3
```




```output1
4
5
```



## Note

<p>In the first example, the answer is $4$.</p><p>The good subsegments are:</p><p>[1]</p><p>[2]</p><p>[3]</p><p>[1, 2]</p><p>In the second example, the answer is $5$.</p><p>The good subsegments are:</p><p>[1]</p><p>[2]</p><p>[3]</p><p>[4]</p><p>[3, 4]</p>
