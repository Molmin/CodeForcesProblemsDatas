## Description

<div><p>You are given $n$ numbers $a_1, a_2, \dots, a_n$. In one operation we can add to any one of those numbers a nonnegative integer power of $2$.</p><p>What is the smallest number of operations we need to perform to make all $n$ numbers equal? It can be proved that under given constraints it doesn't exceed $10^{18}$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^{17}$).</p></div><div class="output-specification"><p>Output exactly one integer&nbsp;— the smallest number of operations we need to perform to make all $n$ numbers equal.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^{17}$).</p>

## Output

<p>Output exactly one integer&nbsp;— the smallest number of operations we need to perform to make all $n$ numbers equal.</p>





```input1
4
228 228 228 228
```




```input2
3
2 2 8
```




```output1
0
```




```output2
3
```



## Note

<p>In the first example, all numbers are already equal. So the needed number of operation is $0$.</p><p>In the second example, we can apply the operation $3$ times: add $8$ to first $2$, add $8$ to second $2$, add $2$ to $8$, making all numbers equal to $10$. It can be proved that we can't make all numbers equal in less than $3$ operations.</p>
