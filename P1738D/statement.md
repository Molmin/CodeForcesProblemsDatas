## Description

<div><p>Given a permutation $a_1, a_2, \dots, a_n$ of integers from $1$ to $n$, and a threshold $k$ with $0 \leq k \leq n$, you compute a sequence $b_1, b_2, \dots, b_n$ as follows. </p><p>For every $1 \leq i \leq n$ in increasing order, let $x = a_i$. </p><ul> <li> If $x \leq k$, set $b_{x}$ to the last element $a_j$ ($1 \leq j &lt; i$) that $a_j &gt; k$. If no such element $a_j$ exists, set $b_{x} = n+1$. </li><li> If $x &gt; k$, set $b_{x}$ to the last element $a_j$ ($1 \leq j &lt; i$) that $a_j \leq k$. If no such element $a_j$ exists, set $b_{x} = 0$. </li></ul><p>Unfortunately, after the sequence $b_1, b_2, \dots, b_n$ has been completely computed, the permutation $a_1, a_2, \dots, a_n$ and the threshold $k$ are discarded. </p><p>Now you only have the sequence $b_1, b_2, \dots, b_n$. Your task is to find any possible permutation $a_1, a_2, \dots, a_n$ and threshold $k$ that produce the sequence $b_1, b_2, \dots, b_n$. <span class="tex-font-style-bf">It is guaranteed that</span> there exists at least one pair of permutation $a_1, a_2, \dots, a_n$ and threshold $k$ that produce the sequence $b_1, b_2, \dots, b_n$.</p><p>A permutation of integers from $1$ to $n$ is a sequence of length $n$ which contains all integers from $1$ to $n$ exactly once. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$), indicating the length of the permutation $a$.</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \leq b_i \leq n+1$), indicating the elements of the sequence $b$.</p><p><span class="tex-font-style-bf">It is guaranteed that</span> there exists at least one pair of permutation $a_1, a_2, \dots, a_n$ and threshold $k$ that produce the sequence $b_1, b_2, \dots, b_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output the threshold $k$ ($0 \leq k \leq n$) in the first line, and then output the permutation $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$) in the second line such that the permutation $a_1, a_2, \dots, a_n$ and threshold $k$ produce the sequence $b_1, b_2, \dots, b_n$. If there are multiple solutions, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$), indicating the length of the permutation $a$.</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \leq b_i \leq n+1$), indicating the elements of the sequence $b$.</p><p><span class="tex-font-style-bf">It is guaranteed that</span> there exists at least one pair of permutation $a_1, a_2, \dots, a_n$ and threshold $k$ that produce the sequence $b_1, b_2, \dots, b_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output the threshold $k$ ($0 \leq k \leq n$) in the first line, and then output the permutation $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$) in the second line such that the permutation $a_1, a_2, \dots, a_n$ and threshold $k$ produce the sequence $b_1, b_2, \dots, b_n$. If there are multiple solutions, you can output any of them.</p>





```input1|2,3,6,7
3
4
5 3 1 2
6
7 7 7 3 3 3
6
4 4 4 0 0 0
```




```output1
2
1 3 2 4
3
1 2 3 4 5 6
3
6 5 4 3 2 1
```



## Note

<p>For the first test case, permutation $a = [1,3,2,4]$ and threshold $k = 2$ will produce sequence $b$ as follows. </p><ul> <li> When $i = 1$, $x = a_i = 1 \leq k$, there is no $a_j$ ($1 \leq j &lt; i$) that $a_j &gt; k$. Therefore, $b_1 = n + 1 = 5$. </li><li> When $i = 2$, $x = a_i = 3 &gt; k$, the last element $a_j$ that $a_j \leq k$ is $a_1$. Therefore, $b_3 = a_1 = 1$. </li><li> When $i = 3$, $x = a_i = 2 \leq k$, the last element $a_j$ that $a_j &gt; k$ is $a_2$. Therefore, $b_2 = a_2 = 3$. </li><li> When $i = 4$, $x = a_i = 4 &gt; k$, the last element $a_j$ that $a_j \leq k$ is $a_3$. Therefore, $b_4 = a_3 = 2$. </li></ul> Finally, we obtain sequence $b = [5,3,1,2]$. <p>For the second test case, permutation $a = [1,2,3,4,5,6]$ and threshold $k = 3$ will produce sequence $b$ as follows. </p><ul> <li> When $i = 1, 2, 3$, $a_i \leq k$, there is no $a_j$ ($1 \leq j &lt; i$) that $a_j &gt; k$. Therefore, $b_1 = b_2 = b_3 = n + 1 = 7$. </li><li> When $i = 4, 5, 6$, $a_i &gt; k$, the last element $a_j$ that $a_j \leq k$ is $a_3$. Therefore, $b_4 = b_5 = b_6 = a_3 = 3$. </li></ul> Finally, we obtain sequence $b = [7,7,7,3,3,3]$. <p>For the third test case, permutation $a = [6,5,4,3,2,1]$ and threshold $k = 3$ will produce sequence $b$ as follows. </p><ul> <li> When $i = 1, 2, 3$, $a_i &gt; k$, there is no $a_j$ ($1 \leq j &lt; i$) that $a_j \leq k$. Therefore, $b_4 = b_5 = b_6 = 0$. </li><li> When $i = 4, 5, 6$, $a_i \leq k$, the last element $a_j$ that $a_j &gt; k$ is $a_3$. Therefore, $b_1 = b_2 = b_3 = a_3 = 4$. </li></ul> Finally, we obtain sequence $b = [4,4,4,0,0,0]$.
