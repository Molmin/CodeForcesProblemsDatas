## Description

<div><p>You are given a positive integer $n$. Your task is to find <span class="tex-font-style-bf">any</span> three integers $a$, $b$ and $c$ ($0 \le a, b, c \le 10^9$) for which $(a\oplus b)+(b\oplus c)+(a\oplus c)=n$, or determine that there are no such integers.</p><p>Here $a \oplus b$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of $a$ and $b$. For example, $2 \oplus 4 = 6$ and $3 \oplus 1=2$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^9$). </p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-bf">any</span> three integers $a$, $b$ and $c$ ($0 \le a, b, c \le 10^9$) for which $(a\oplus b)+(b\oplus c)+(a\oplus c)=n$. If no such integers exist, print $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^9$). </p>

## Output

<p>For each test case, print <span class="tex-font-style-bf">any</span> three integers $a$, $b$ and $c$ ($0 \le a, b, c \le 10^9$) for which $(a\oplus b)+(b\oplus c)+(a\oplus c)=n$. If no such integers exist, print $-1$.</p>





```input1|2,4,6
5
4
1
12
2046
194723326
```




```output1
3 3 1
-1
2 4 6
69 420 666
12345678 87654321 100000000
```



## Note

<p>In the first test case, $a=3$, $b=3$, $c=1$, so $(3 \oplus 3)+(3 \oplus 1) + (3 \oplus 1)=0+2+2=4$.</p><p>In the second test case, there are no solutions.</p><p>In the third test case, $(2 \oplus 4)+(4 \oplus 6) + (2 \oplus 6)=6+2+4=12$.</p>
