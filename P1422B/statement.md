## Description

<div><p>A matrix of size $n \times m$ is called nice, if all rows and columns of the matrix are palindromes. A sequence of integers $(a_1, a_2, \dots , a_k)$ is a palindrome, if for any integer $i$ ($1 \le i \le k$) the equality $a_i = a_{k - i + 1}$ holds.</p><p>Sasha owns a matrix $a$ of size $n \times m$. In one operation he can increase or decrease any number in the matrix by one. Sasha wants to make the matrix nice. He is interested what is the minimum number of operations he needs.</p><p>Help him!</p></div><div class="input-specification"><p>The first line contains a single integer $t$&nbsp;— the number of test cases ($1 \le t \le 10$). The $t$ tests follow.</p><p>The first line of each test contains two integers $n$ and $m$ ($1 \le n, m \le 100$)&nbsp;— the size of the matrix.</p><p>Each of the next $n$ lines contains $m$ integers $a_{i, j}$ ($0 \le a_{i, j} \le 10^9$)&nbsp;— the elements of the matrix.</p></div><div class="output-specification"><p>For each test output the smallest number of operations required to make the matrix nice.</p></div>

## Input

<p>The first line contains a single integer $t$&nbsp;— the number of test cases ($1 \le t \le 10$). The $t$ tests follow.</p><p>The first line of each test contains two integers $n$ and $m$ ($1 \le n, m \le 100$)&nbsp;— the size of the matrix.</p><p>Each of the next $n$ lines contains $m$ integers $a_{i, j}$ ($0 \le a_{i, j} \le 10^9$)&nbsp;— the elements of the matrix.</p>

## Output

<p>For each test output the smallest number of operations required to make the matrix nice.</p>





```input1
2
4 2
4 2
2 4
4 2
2 4
3 4
1 2 3 4
5 6 7 8
9 10 11 18
```




```output1
8
42
```



## Note

<p>In the first test case we can, for example, obtain the following nice matrix in $8$ operations:</p><pre class="verbatim"><br>2 2<br>4 4<br>4 4<br>2 2<br></pre><p>In the second test case we can, for example, obtain the following nice matrix in $42$ operations:</p><pre class="verbatim"><br>5 6 6 5<br>6 6 6 6<br>5 6 6 5<br></pre>
