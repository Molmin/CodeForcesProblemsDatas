## Description

<div><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). There are $n! = n \cdot (n-1) \cdot (n - 2) \cdot \ldots \cdot 1$ different permutations of length $n$.</p><p>Given a permutation $p$ of $n$ numbers, we create an array $a$ consisting of $2n$ numbers, which is equal to $p$ concatenated with its reverse. We then define the beauty of $p$ as the number of inversions in $a$.</p><p>The number of inversions in the array $a$ is the number of pairs of indices $i$, $j$ such that $i &lt; j$ and $a_i &gt; a_j$.</p><p>For example, for permutation $p = [1, 2]$, $a$ would be $[1, 2, 2, 1]$. The inversions in $a$ are $(2, 4)$ and $(3, 4)$ (assuming 1-based indexing). Hence, the beauty of $p$ is $2$.</p><p>Your task is to find the sum of beauties of all $n!$ permutations of size $n$. Print the remainder we get when dividing this value by $1\,000\,000\,007$ ($10^9 + 7$).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>Each test case has only one line — the integer $n$ ($1 \leq n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer — the sum of beauties of all permutations of size $n$ modulo $1\,000\,000\,007$ ($10^9 + 7$).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>Each test case has only one line — the integer $n$ ($1 \leq n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print one integer — the sum of beauties of all permutations of size $n$ modulo $1\,000\,000\,007$ ($10^9 + 7$).</p>





```input1|2,4
3
1
2
100
```




```output1
0
4
389456655
```



## Note

<p>For the first test case of the example, $p = [1]$ is the only permutation. $a = [1, 1]$ has $0$ inversions.</p><p>For the second test case of the example, the permutations are $[1, 2]$ and $[2, 1]$. Their respective $a$ arrays are $[1, 2, 2, 1]$ and $[2, 1, 1, 2]$, both of which have $2$ inversions.</p>
