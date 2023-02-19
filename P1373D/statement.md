## Description

<div><p>You are given an array $a$ consisting of $n$ integers. Indices of the array start from zero (i. e. the first element is $a_0$, the second one is $a_1$, and so on).</p><p>You can reverse <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of this array. Recall that the subarray of $a$ with borders $l$ and $r$ is $a[l; r] = a_l, a_{l + 1}, \dots, a_{r}$.</p><p>Your task is to reverse such a subarray that the sum of elements on <span class="tex-font-style-bf">even</span> positions of the resulting array is <span class="tex-font-style-bf">maximized</span> (i. e. the sum of elements $a_0, a_2, \dots, a_{2k}$ for integer $k = \lfloor\frac{n-1}{2}\rfloor$ should be maximum possible).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_0, a_1, \dots, a_{n-1}$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer on the separate line — the <span class="tex-font-style-bf">maximum</span> possible sum of elements on <span class="tex-font-style-bf">even</span> positions after reversing <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of $a$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_0, a_1, \dots, a_{n-1}$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer on the separate line — the <span class="tex-font-style-bf">maximum</span> possible sum of elements on <span class="tex-font-style-bf">even</span> positions after reversing <span class="tex-font-style-bf">at most one</span> subarray (continuous subsegment) of $a$.</p>





```input1
4
8
1 7 3 4 7 6 2 9
5
1 2 1 2 1
10
7 8 4 5 7 6 8 9 7 3
4
3 1 2 1
```




```output1
26
5
37
5
```


