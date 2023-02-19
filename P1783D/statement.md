## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>You <span class="tex-font-style-bf">have to</span> perform the sequence of $n-2$ operations on this array:</p><ul> <li> during the first operation, you either add $a_2$ to $a_1$ and subtract $a_2$ from $a_3$, or add $a_2$ to $a_3$ and subtract $a_2$ from $a_1$; </li><li> during the second operation, you either add $a_3$ to $a_2$ and subtract $a_3$ from $a_4$, or add $a_3$ to $a_4$ and subtract $a_3$ from $a_2$; </li><li> ... </li><li> during the last operation, you either add $a_{n-1}$ to $a_{n-2}$ and subtract $a_{n-1}$ from $a_n$, or add $a_{n-1}$ to $a_n$ and subtract $a_{n-1}$ from $a_{n-2}$. </li></ul><p>So, during the $i$-th operation, you add the value of $a_{i+1}$ to one of its neighbors, and subtract it from the other neighbor.</p><p>For example, if you have the array $[1, 2, 3, 4, 5]$, one of the possible sequences of operations is:</p><ul> <li> subtract $2$ from $a_3$ and add it to $a_1$, so the array becomes $[3, 2, 1, 4, 5]$; </li><li> subtract $1$ from $a_2$ and add it to $a_4$, so the array becomes $[3, 1, 1, 5, 5]$; </li><li> subtract $5$ from $a_3$ and add it to $a_5$, so the array becomes $[3, 1, -4, 5, 10]$. </li></ul><p>So, the resulting array is $[3, 1, -4, 5, 10]$.</p><p>An array is <span class="tex-font-style-it">reachable</span> if it can be obtained by performing the aforementioned sequence of operations on $a$. You have to calculate the number of reachable arrays, and print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($3 \le n \le 300$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 300$).</p></div><div class="output-specification"><p>Print one integer — the number of reachable arrays. Since the answer can be very large, print its remainder modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($3 \le n \le 300$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 300$).</p>

## Output

<p>Print one integer — the number of reachable arrays. Since the answer can be very large, print its remainder modulo $998244353$.</p>





```input1
4
1 1 1 1
```




```input2
5
1 2 3 5 0
```




```output1
3
```




```output2
7
```


