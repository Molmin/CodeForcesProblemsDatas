## Description

<div><p>Today, as a friendship gift, Bakry gave Badawy $n$ integers $a_1, a_2, \dots, a_n$ and challenged him to choose an integer $X$ such that the value $\underset{1 \leq i \leq n}{\max} (a_i \oplus X)$ is minimum possible, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>As always, Badawy is too lazy, so you decided to help him and find the minimum possible value of $\underset{1 \leq i \leq n}{\max} (a_i \oplus X)$.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($1\le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^{30}-1$).</p></div><div class="output-specification"><p>Print one integer — the minimum possible value of $\underset{1 \leq i \leq n}{\max} (a_i \oplus X)$.</p></div>

## Input

<p>The first line contains integer $n$ ($1\le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^{30}-1$).</p>

## Output

<p>Print one integer — the minimum possible value of $\underset{1 \leq i \leq n}{\max} (a_i \oplus X)$.</p>





```input1
3
1 2 3
```




```input2
2
1 5
```




```output1
2
```




```output2
4
```



## Note

<p>In the first sample, we can choose $X = 3$.</p><p>In the second sample, we can choose $X = 5$.</p>
