## Description

<div><p>You are given an array $a$ consisting of $n$ integers. You have to find the length of the smallest (shortest) <span class="tex-font-style-it">prefix</span> of elements you need to erase from $a$ to make it a <span class="tex-font-style-it">good</span> array. Recall that the prefix of the array $a=[a_1, a_2, \dots, a_n]$ is a subarray consisting several first elements: the prefix of the array $a$ of length $k$ is the array $[a_1, a_2, \dots, a_k]$ ($0 \le k \le n$).</p><p>The array $b$ of length $m$ is called <span class="tex-font-style-it">good</span>, if you can obtain a <span class="tex-font-style-bf">non-decreasing</span> array $c$ ($c_1 \le c_2 \le \dots \le c_{m}$) from it, repeating the following operation $m$ times (initially, $c$ is empty):</p><ul> <li> select either the first or the last element of $b$, remove it from $b$, and append it to the end of the array $c$. </li></ul><p>For example, if we do $4$ operations: take $b_1$, then $b_{m}$, then $b_{m-1}$ and at last $b_2$, then $b$ becomes $[b_3, b_4, \dots, b_{m-3}]$ and $c =[b_1, b_{m}, b_{m-1}, b_2]$.</p><p>Consider the following example: $b = [1, 2, 3, 4, 4, 2, 1]$. This array is <span class="tex-font-style-bf">good</span> because we can obtain <span class="tex-font-style-bf">non-decreasing</span> array $c$ from it by the following sequence of operations:</p><ol> <li> take the first element of $b$, so $b = [2, 3, 4, 4, 2, 1]$, $c = [1]$; </li><li> take the last element of $b$, so $b = [2, 3, 4, 4, 2]$, $c = [1, 1]$; </li><li> take the last element of $b$, so $b = [2, 3, 4, 4]$, $c = [1, 1, 2]$; </li><li> take the first element of $b$, so $b = [3, 4, 4]$, $c = [1, 1, 2, 2]$; </li><li> take the first element of $b$, so $b = [4, 4]$, $c = [1, 1, 2, 2, 3]$; </li><li> take the last element of $b$, so $b = [4]$, $c = [1, 1, 2, 2, 3, 4]$; </li><li> take the only element of $b$, so $b = []$, $c = [1, 1, 2, 2, 3, 4, 4]$&nbsp;— $c$ is non-decreasing. </li></ol><p>Note that the array consisting of one element is <span class="tex-font-style-it">good</span>.</p><p>Print the length of the shortest prefix of $a$ to delete (erase), to make $a$ to be a <span class="tex-font-style-it">good</span> array. Note that the required length can be $0$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer: the length of the shortest <span class="tex-font-style-it">prefix</span> of elements you need to erase from $a$ to make it a <span class="tex-font-style-it">good</span> array.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer: the length of the shortest <span class="tex-font-style-it">prefix</span> of elements you need to erase from $a$ to make it a <span class="tex-font-style-it">good</span> array.</p>





```input1
5
4
1 2 3 4
7
4 3 3 8 4 5 2
3
1 1 1
7
1 3 1 4 5 3 2
5
5 4 3 2 3
```




```output1
0
4
0
2
3
```



## Note

<p>In the first test case of the example, the array $a$ is already good, so we don't need to erase any prefix.</p><p>In the second test case of the example, the initial array $a$ is not good. Let's erase first $4$ elements of $a$, the result is $[4, 5, 2]$. The resulting array is good. You can prove that if you erase fewer number of first elements, the result will not be good.</p>
