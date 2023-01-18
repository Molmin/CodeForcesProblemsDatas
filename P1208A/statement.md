## Description

<div><p>Cengiz recently learned Fibonacci numbers and now he is studying different algorithms to find them. After getting bored of reading them, he came with his own new type of numbers that he named <span class="tex-font-style-it">XORinacci</span> numbers. He defined them as follows: </p><ul> <li> $f(0) = a$; </li><li> $f(1) = b$; </li><li> $f(n) = f(n-1) \oplus f(n-2)$ when $n &gt; 1$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </li></ul><p>You are given three integers $a$, $b$, and $n$, calculate $f(n)$.</p><p>You have to answer for $T$ independent test cases.</p></div><div class="input-specification"><p>The input contains one or more independent test cases.</p><p>The first line of input contains a single integer $T$ ($1 \le T \le 10^3$), the number of test cases.</p><p>Each of the $T$ following lines contains three space-separated integers $a$, $b$, and $n$ ($0 \le a, b, n \le 10^9$) respectively.</p></div><div class="output-specification"><p>For each test case, output $f(n)$.</p></div>

## Input

<p>The input contains one or more independent test cases.</p><p>The first line of input contains a single integer $T$ ($1 \le T \le 10^3$), the number of test cases.</p><p>Each of the $T$ following lines contains three space-separated integers $a$, $b$, and $n$ ($0 \le a, b, n \le 10^9$) respectively.</p>

## Output

<p>For each test case, output $f(n)$.</p>





```input1
3
3 4 2
4 5 0
325 265 1231232
```




```output1
7
4
76
```



## Note

<p>In the first example, $f(2) = f(0) \oplus f(1) = 3 \oplus 4 = 7$.</p>
