## Description

<div><p>Jeevan has two arrays $a$ and $b$ of size $n$. He is fond of performing weird operations on arrays. This time, he comes up with two types of operations:</p><ul> <li> Choose any $i$ ($1 \le i \le n$) and increment $a_j$ by $1$ for every $j$ which is a multiple of $i$ and $1 \le j \le n$. </li><li> Choose any $i$ ($1 \le i \le n$) and decrement $a_j$ by $1$ for every $j$ which is a multiple of $i$ and $1 \le j \le n$. </li></ul><p>He wants to convert array $a$ into an array $b$ using the minimum total number of operations. However, Jeevan seems to have forgotten the value of $b_1$. So he makes some guesses. He will ask you $q$ questions corresponding to his $q$ guesses, the $i$-th of which is of the form: </p><ul> <li> If $b_1 = x_i$, what is the minimum number of operations required to convert $a$ to $b$? </li></ul><p>Help him by answering each question.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ &nbsp;— the size of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \le a_i \le 10^6)$.</p><p>The third line contains $n$ integers $b_1, b_2, ..., b_n$ $(1 \le b_i \le 10^6$ for $i \neq 1$; $b_1 = -1$, representing that the value of $b_1$ is unknown$)$.</p><p>The fourth line contains a single integer $q$ $(1 \le q \le 2 \cdot 10^{5})$ &nbsp;— the number of questions.</p><p>Each of the following $q$ lines contains a single integer $x_i$ $(1 \le x_i \le 10^6)$ &nbsp;— representing the $i$-th question.</p></div><div class="output-specification"><p>Output $q$ integers &nbsp;— the answers to each of his $q$ questions.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ &nbsp;— the size of arrays $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \le a_i \le 10^6)$.</p><p>The third line contains $n$ integers $b_1, b_2, ..., b_n$ $(1 \le b_i \le 10^6$ for $i \neq 1$; $b_1 = -1$, representing that the value of $b_1$ is unknown$)$.</p><p>The fourth line contains a single integer $q$ $(1 \le q \le 2 \cdot 10^{5})$ &nbsp;— the number of questions.</p><p>Each of the following $q$ lines contains a single integer $x_i$ $(1 \le x_i \le 10^6)$ &nbsp;— representing the $i$-th question.</p>

## Output

<p>Output $q$ integers &nbsp;— the answers to each of his $q$ questions.</p>





```input1
2
3 7
-1 5
3
1
4
3
```




```input2
6
2 5 4 1 3 6
-1 4 6 2 3 5
3
1
8
4
```




```output1
2
4
2
```




```output2
10
29
9
```



## Note

<p>Consider the first test case.</p><ul> <li> $b_1 = 1$: We need to convert $[3, 7] \rightarrow [1, 5]$. We can perform the following operations:<p>$[3, 7]$ $\xrightarrow[\text{decrease}]{\text{i = 1}}$ $[2, 6]$ $\xrightarrow[\text{decrease}]{\text{i = 1}}$ $[1, 5]$</p><p>Hence the answer is $2$.</p></li><li> $b_1 = 4$: We need to convert $[3, 7] \rightarrow [4, 5]$. We can perform the following operations: <p>$[3, 7]$ $\xrightarrow[\text{decrease}]{\text{i = 2}}$ $[3, 6]$ $\xrightarrow[\text{decrease}]{\text{i = 2}}$ $[3, 5]$ $\xrightarrow[\text{increase}]{\text{i = 1}}$ $[4, 6]$ $\xrightarrow[\text{decrease}]{\text{i = 2}}$ $[4, 5]$</p><p>Hence the answer is $4$.</p></li><li> $b_1 = 3$: We need to convert $[3, 7] \rightarrow [3, 5]$. We can perform the following operations:<p>$[3, 7]$ $\xrightarrow[\text{decrease}]{\text{i = 2}}$ $[3, 6]$ $\xrightarrow[\text{decrease}]{\text{i = 2}}$ $[3, 5]$</p><p>Hence the answer is $2$.</p></li></ul>
