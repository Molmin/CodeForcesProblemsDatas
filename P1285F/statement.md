## Description

<div><p>Given an array $a$, consisting of $n$ integers, find:</p><p>$$\max\limits_{1 \le i &lt; j \le n} LCM(a_i,a_j),$$</p><p>where $LCM(x, y)$ is the smallest positive integer that is divisible by both $x$ and $y$. For example, $LCM(6, 8) = 24$, $LCM(4, 12) = 12$, $LCM(2, 3) = 6$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>Print one integer, the maximum value of the least common multiple of two elements in the array $a$.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>Print one integer, the maximum value of the least common multiple of two elements in the array $a$.</p>





```input1
3
13 35 77
```




```input2
6
1 2 4 8 16 32
```




```output1
1001
```




```output2
32
```


