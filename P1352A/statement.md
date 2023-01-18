## Description

<div><p>A positive (strictly greater than zero) integer is called <span class="tex-font-style-it">round</span> if it is of the form <span class="tex-font-style-tt">d00...0</span>. In other words, a positive integer is round if all its digits except the leftmost (most significant) are equal to zero. In particular, all numbers from $1$ to $9$ (inclusive) are round.</p><p>For example, the following numbers are round: $4000$, $1$, $9$, $800$, $90$. The following numbers are <span class="tex-font-style-bf">not</span> round: $110$, $707$, $222$, $1001$.</p><p>You are given a positive integer $n$ ($1 \le n \le 10^4$). Represent the number $n$ as a sum of round numbers using the minimum number of summands (addends). In other words, you need to represent the given number $n$ as a sum of the least number of terms, each of which is a round number.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is a line containing an integer $n$ ($1 \le n \le 10^4$).</p></div><div class="output-specification"><p>Print $t$ answers to the test cases. Each answer must begin with an integer $k$ — the minimum number of summands. Next, $k$ terms must follow, each of which is a round number, and their sum is $n$. The terms can be printed in any order. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is a line containing an integer $n$ ($1 \le n \le 10^4$).</p>

## Output

<p>Print $t$ answers to the test cases. Each answer must begin with an integer $k$ — the minimum number of summands. Next, $k$ terms must follow, each of which is a round number, and their sum is $n$. The terms can be printed in any order. If there are several answers, print any of them.</p>





```input1
5
5009
7
9876
10000
10
```




```output1
2
5000 9
1
7 
4
800 70 6 9000 
1
10000 
1
10
```


