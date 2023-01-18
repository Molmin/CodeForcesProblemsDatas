## Description

<div><p>You are given an array $a$ consisting of $n$ elements. You may apply several operations (possibly zero) to it.</p><p>During each operation, you choose two indices $i$ and $j$ ($1 \le i, j \le n$; $i \ne j$), increase $a_j$ by $a_i$, and remove the $i$-th element from the array (so the indices of all elements to the right to it decrease by $1$, and $n$ also decreases by $1$).</p><p>Your goal is to make the array $a$ strictly ascending. That is, the condition $a_1 &lt; a_2 &lt; \dots &lt; a_n$ should hold (where $n$ is the resulting size of the array).</p><p>Calculate the minimum number of actions required to make the array strictly ascending.</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 10000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($1 \le n \le 15$) — the number of elements in the initial array $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that: </p><ul> <li> the number of test cases having $n \ge 5$ is not greater than $5000$; </li><li> the number of test cases having $n \ge 8$ is not greater than $500$; </li><li> the number of test cases having $n \ge 10$ is not greater than $100$; </li><li> the number of test cases having $n \ge 11$ is not greater than $50$; </li><li> the number of test cases having $n \ge 12$ is not greater than $25$; </li><li> the number of test cases having $n \ge 13$ is not greater than $10$; </li><li> the number of test cases having $n \ge 14$ is not greater than $3$; </li><li> the number of test cases having $n \ge 15$ is not greater than $1$. </li></ul></div><div class="output-specification"><p>For each test case, print the answer as follows:</p><p>In the first line, print $k$ — the minimum number of operations you have to perform. Then print $k$ lines, each containing two indices $i$ and $j$ for the corresponding operation. Note that the numeration of elements in the array changes after removing elements from it. If there are multiple optimal sequences of operations, print any one of them.</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 10000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($1 \le n \le 15$) — the number of elements in the initial array $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that: </p><ul> <li> the number of test cases having $n \ge 5$ is not greater than $5000$; </li><li> the number of test cases having $n \ge 8$ is not greater than $500$; </li><li> the number of test cases having $n \ge 10$ is not greater than $100$; </li><li> the number of test cases having $n \ge 11$ is not greater than $50$; </li><li> the number of test cases having $n \ge 12$ is not greater than $25$; </li><li> the number of test cases having $n \ge 13$ is not greater than $10$; </li><li> the number of test cases having $n \ge 14$ is not greater than $3$; </li><li> the number of test cases having $n \ge 15$ is not greater than $1$. </li></ul>

## Output

<p>For each test case, print the answer as follows:</p><p>In the first line, print $k$ — the minimum number of operations you have to perform. Then print $k$ lines, each containing two indices $i$ and $j$ for the corresponding operation. Note that the numeration of elements in the array changes after removing elements from it. If there are multiple optimal sequences of operations, print any one of them.</p>





```input1
4
8
2 1 3 5 1 2 4 5
15
16384 8192 4096 2048 1024 512 256 128 64 32 16 8 4 2 1
2
3 3
14
1 2 3 4 5 6 7 8 9 10 11 12 13 14
```




```output1
3
6 8
1 6
4 1
7
1 15
1 13
1 11
1 9
1 7
1 5
1 3
1
2 1
0
```



## Note

<p>In the first test case, the sequence of operations changes $a$ as follows:</p><p>$[2, 1, 3, 5, 1, 2, 4, 5] \rightarrow [2, 1, 3, 5, 1, 4, 7] \rightarrow [1, 3, 5, 1, 6, 7] \rightarrow [2, 3, 5, 6, 7]$.</p>
