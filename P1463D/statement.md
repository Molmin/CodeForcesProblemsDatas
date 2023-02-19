## Description

<div><p>You have $2n$ integers $1, 2, \dots, 2n$. You have to redistribute these $2n$ elements into $n$ pairs. After that, you choose $x$ pairs and take minimum elements from them, and from the other $n - x$ pairs, you take maximum elements.</p><p>Your goal is to obtain the set of numbers $\{b_1, b_2, \dots, b_n\}$ as the result of taking elements from the pairs.</p><p>What is the number of different $x$-s ($0 \le x \le n$) such that it's possible to obtain the set $b$ if for each $x$ you can choose how to distribute numbers into pairs and from which $x$ pairs choose minimum elements?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_1 &lt; b_2 &lt; \dots &lt; b_n \le 2n$)&nbsp;— the set you'd like to get.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one number&nbsp;— the number of different $x$-s such that it's possible to obtain the set $b$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_1 &lt; b_2 &lt; \dots &lt; b_n \le 2n$)&nbsp;— the set you'd like to get.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one number&nbsp;— the number of different $x$-s such that it's possible to obtain the set $b$.</p>





```input1
3
1
1
5
1 4 5 9 10
2
3 4
```




```output1
1
3
1
```



## Note

<p>In the first test case, $x = 1$ is the only option: you have one pair $(1, 2)$ and choose the minimum from this pair.</p><p>In the second test case, there are three possible $x$-s. If $x = 1$, then you can form the following pairs: $(1, 6)$, $(2, 4)$, $(3, 5)$, $(7, 9)$, $(8, 10)$. You can take minimum from $(1, 6)$ (equal to $1$) and the maximum elements from all other pairs to get set $b$.</p><p>If $x = 2$, you can form pairs $(1, 2)$, $(3, 4)$, $(5, 6)$, $(7, 9)$, $(8, 10)$ and take the minimum elements from $(1, 2)$, $(5, 6)$ and the maximum elements from the other pairs.</p><p>If $x = 3$, you can form pairs $(1, 3)$, $(4, 6)$, $(5, 7)$, $(2, 9)$, $(8, 10)$ and take the minimum elements from $(1, 3)$, $(4, 6)$, $(5, 7)$.</p><p>In the third test case, $x = 0$ is the only option: you can form pairs $(1, 3)$, $(2, 4)$ and take the maximum elements from both of them.</p>
