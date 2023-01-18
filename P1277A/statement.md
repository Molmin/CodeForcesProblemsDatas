## Description

<div><p>Hooray! Polycarp turned $n$ years old! The Technocup Team sincerely congratulates Polycarp!</p><p>Polycarp celebrated all of his $n$ birthdays: from the $1$-th to the $n$-th. At the moment, he is wondering: how many times he turned <span class="tex-font-style-it">beautiful</span> number of years?</p><p>According to Polycarp, a positive integer is <span class="tex-font-style-it">beautiful</span> if it consists of only one digit repeated one or more times. For example, the following numbers are beautiful: $1$, $77$, $777$, $44$ and $999999$. The following numbers are not beautiful: $12$, $11110$, $6969$ and $987654321$.</p><p>Of course, Polycarpus uses the decimal numeral system (i.e. radix is 10).</p><p>Help Polycarpus to find the number of numbers from $1$ to $n$ (inclusive) that are beautiful.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case consists of one line, which contains a positive integer $n$ ($1 \le n \le 10^9$) — how many years Polycarp has turned.</p></div><div class="output-specification"><p>Print $t$ integers — the answers to the given test cases in the order they are written in the test. Each answer is an integer: the number of beautiful years between $1$ and $n$, inclusive.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case consists of one line, which contains a positive integer $n$ ($1 \le n \le 10^9$) — how many years Polycarp has turned.</p>

## Output

<p>Print $t$ integers — the answers to the given test cases in the order they are written in the test. Each answer is an integer: the number of beautiful years between $1$ and $n$, inclusive.</p>





```input1
6
18
1
9
100500
33
1000000000
```




```output1
10
1
9
45
12
81
```



## Note

<p>In the first test case of the example beautiful years are $1$, $2$, $3$, $4$, $5$, $6$, $7$, $8$, $9$ and $11$.</p>
