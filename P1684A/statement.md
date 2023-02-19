## Description

<div><p>There is an integer $n$ <span class="tex-font-style-bf">without zeros</span> in its decimal representation. Alice and Bob are playing a game with this integer. Alice starts first. They play the game in turns.</p><p>On her turn, Alice <span class="tex-font-style-bf">must</span> swap any two digits of the integer that are on different positions. Bob on his turn always removes the last digit of the integer. The game ends when there is only one digit left.</p><p>You have to find the smallest integer Alice can get in the end, if she plays optimally.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains the integer $n$ ($10 \le n \le 10^9$) — the integer for the game. $n$ does not have zeros in its decimal representation.</p></div><div class="output-specification"><p>For each test case output a single integer — the smallest integer Alice can get in the end of the game.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains the integer $n$ ($10 \le n \le 10^9$) — the integer for the game. $n$ does not have zeros in its decimal representation.</p>

## Output

<p>For each test case output a single integer — the smallest integer Alice can get in the end of the game.</p>





```input1
3
12
132
487456398
```




```output1
2
1
3
```



## Note

<p>In the first test case Alice has to swap $1$ and $2$. After that Bob removes the last digit, $1$, so the answer is $2$.</p><p>In the second test case Alice can swap $3$ and $1$: $312$. After that Bob deletes the last digit: $31$. Then Alice swaps $3$ and $1$: $13$ and Bob deletes $3$, so the answer is $1$.</p>
