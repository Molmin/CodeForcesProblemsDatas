## Description

<div><p>You are given a number $n$ and an array $b_1, b_2, \ldots, b_{n+2}$, obtained according to the following algorithm: </p><ul> <li> some array $a_1, a_2, \ldots, a_n$ was guessed; </li><li> array $a$ was written to array $b$, i.e. $b_i = a_i$ ($1 \le i \le n$); </li><li> The $(n+1)$-th element of the array $b$ is the sum of the numbers in the array $a$, i.e. $b_{n+1} = a_1+a_2+\ldots+a_n$; </li><li> The $(n+2)$-th element of the array $b$ was written some number $x$ ($1 \le x \le 10^9$), i.e. $b_{n+2} = x$; The </li><li> array $b$ was shuffled. </li></ul><p>For example, the array $b=[2, 3, 7, 12 ,2]$ it could be obtained in the following ways: </p><ul> <li> $a=[2, 2, 3]$ and $x=12$; </li><li> $a=[3, 2, 7]$ and $x=2$. </li></ul><p>For the given array $b$, find any array $a$ that could have been guessed initially.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second row of each test case contains $n+2$ integers $b_1, b_2, \ldots, b_{n+2}$ ($1 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>", if the array $b$ could not be obtained from any array $a$; </li><li> $n$ integers $a_1, a_2, \ldots, a_n$, otherwise. </li></ul><p>If there are several arrays of $a$, you can output any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second row of each test case contains $n+2$ integers $b_1, b_2, \ldots, b_{n+2}$ ($1 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>", if the array $b$ could not be obtained from any array $a$; </li><li> $n$ integers $a_1, a_2, \ldots, a_n$, otherwise. </li></ul><p>If there are several arrays of $a$, you can output any.</p>





```input1
4
3
2 3 7 12 2
4
9 1 7 1 6 5
5
18 2 2 3 2 9 2
3
2 6 9 2 1
```




```output1
2 3 7 
-1
2 2 2 3 9 
1 2 6
```


