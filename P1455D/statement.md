## Description

<div><p>You are given a sequence $a$ consisting of $n$ integers $a_1, a_2, \dots, a_n$, and an integer $x$. Your task is to make the sequence $a$ sorted (it is considered sorted if the condition $a_1 \le a_2 \le a_3 \le \dots \le a_n$ holds).</p><p>To make the sequence sorted, you may perform the following operation any number of times you want (possibly zero): choose an integer $i$ such that $1 \le i \le n$ and $a_i &gt; x$, and swap the values of $a_i$ and $x$.</p><p>For example, if $a = [0, 2, 3, 5, 4]$, $x = 1$, the following sequence of operations is possible:</p><ol> <li> choose $i = 2$ (it is possible since $a_2 &gt; x$), then $a = [0, 1, 3, 5, 4]$, $x = 2$; </li><li> choose $i = 3$ (it is possible since $a_3 &gt; x$), then $a = [0, 1, 2, 5, 4]$, $x = 3$; </li><li> choose $i = 4$ (it is possible since $a_4 &gt; x$), then $a = [0, 1, 2, 3, 4]$, $x = 5$. </li></ol><p>Calculate the minimum number of operations you have to perform so that $a$ becomes sorted, or report that it is impossible.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains two integers $n$ and $x$ ($1 \le n \le 500$, $0 \le x \le 500$) — the number of elements in the sequence and the initial value of $x$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_i \le 500$).</p><p>The sum of values of $n$ over all test cases in the input does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of operations you have to perform to make $a$ sorted, or $-1$, if it is impossible.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains two integers $n$ and $x$ ($1 \le n \le 500$, $0 \le x \le 500$) — the number of elements in the sequence and the initial value of $x$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_i \le 500$).</p><p>The sum of values of $n$ over all test cases in the input does not exceed $500$.</p>

## Output

<p>For each test case, print one integer — the minimum number of operations you have to perform to make $a$ sorted, or $-1$, if it is impossible.</p>





```input1
6
4 1
2 3 5 4
5 6
1 1 3 4 4
1 10
2
2 10
11 9
2 10
12 11
5 18
81 324 218 413 324
```




```output1
3
0
0
-1
1
3
```


