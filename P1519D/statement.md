## Description

<div><p>You are given two integer arrays $a$ and $b$ of length $n$.</p><p>You can reverse <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of the array $a$. </p><p>Your task is to reverse such a subarray that the sum $\sum\limits_{i=1}^n a_i \cdot b_i$ is <span class="tex-font-style-bf">maximized</span>.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^7$).</p></div><div class="output-specification"><p>Print single integer — maximum possible sum after reversing <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of $a$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^7$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^7$).</p>

## Output

<p>Print single integer — maximum possible sum after reversing <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of $a$.</p>





```input1
5
2 3 2 1 3
1 3 2 4 2
```




```input2
2
13 37
2 4
```




```input3
6
1 8 7 6 3 6
5 9 6 8 8 6
```




```output1
29
```




```output2
174
```




```output3
235
```



## Note

<p>In the first example, you can reverse the subarray $[4, 5]$. Then $a = [2, 3, 2, 3, 1]$ and $2 \cdot 1 + 3 \cdot 3 + 2 \cdot 2 + 3 \cdot 4 + 1 \cdot 2 = 29$.</p><p>In the second example, you don't need to use the reverse operation. $13 \cdot 2 + 37 \cdot 4 = 174$.</p><p>In the third example, you can reverse the subarray $[3, 5]$. Then $a = [1, 8, 3, 6, 7, 6]$ and $1 \cdot 5 + 8 \cdot 9 + 3 \cdot 6 + 6 \cdot 8 + 7 \cdot 8 + 6 \cdot 6 = 235$.</p>
