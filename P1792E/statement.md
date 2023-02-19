## Description

<div><p>You are given an $n \times n$ multiplication table and a positive integer $m = m_1 \cdot m_2$. A $n \times n$ multiplication table is a table with $n$ rows and $n$ columns numbered from $1$ to $n$, where $a_{i, j} = i \cdot j$.</p><p>For each divisor $d$ of $m$, check: does $d$ occur in the table at least once, and if it does, what is the <span class="tex-font-style-it">minimum</span> row that contains $d$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $m_1$ and $m_2$ ($1 \le n \le 10^9$; $1 \le m_1, m_2 \le 10^9$)&nbsp;— the size of the multiplication table and the integer $m$ represented as $m_1 \cdot m_2$.</p></div><div class="output-specification"><p>For each test case, let $d_1, d_2, \dots, d_k$ be <span class="tex-font-style-it">all</span> divisors of $m$ sorted in the increasing order. And let $a_1, a_2, \dots, a_k$ be an array of answers, where $a_i$ is equal to the minimum row index where divisor $d_i$ occurs, or $0$, if there is no such row.</p><p>Since array $a$ may be large, first, print an integer $s$&nbsp;— the number of divisors of $m$ that <span class="tex-font-style-it">are present</span> in the $n \times n$ table. Next, print a single value $X = a_1 \oplus a_2 \oplus \dots \oplus a_k$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $m_1$ and $m_2$ ($1 \le n \le 10^9$; $1 \le m_1, m_2 \le 10^9$)&nbsp;— the size of the multiplication table and the integer $m$ represented as $m_1 \cdot m_2$.</p>

## Output

<p>For each test case, let $d_1, d_2, \dots, d_k$ be <span class="tex-font-style-it">all</span> divisors of $m$ sorted in the increasing order. And let $a_1, a_2, \dots, a_k$ be an array of answers, where $a_i$ is equal to the minimum row index where divisor $d_i$ occurs, or $0$, if there is no such row.</p><p>Since array $a$ may be large, first, print an integer $s$&nbsp;— the number of divisors of $m$ that <span class="tex-font-style-it">are present</span> in the $n \times n$ table. Next, print a single value $X = a_1 \oplus a_2 \oplus \dots \oplus a_k$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p>





```input1|2,4
3
3 72 1
10 10 15
6 1 210
```




```output1
6 2
10 0
8 5
```



## Note

<p>In the first test case, $m = 72 \cdot 1 = 72$ and has $12$ divisors $[1, 2, 3, 4, 6, 8, 9, 12, 18, 24, 36, 72]$. The $3 \times 3$ multiplication table looks like that:</p><center> <center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">1</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">3</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">2</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">3</span></td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">4</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">6</span></td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">9</span></td></tr></tbody></table> </center> </center><p>For each divisor of $m$ that is present in the table, the position with minimum row index is marked. So the array of answers $a$ is equal to $[1, 1, 1, 2, 2, 0, 3, 0, 0, 0, 0, 0]$. There are only $6$ non-zero values, and xor of $a$ is equal to $2$.</p><p>In the second test case, $m = 10 \cdot 15 = 150$ and has $12$ divisors $[1, 2, 3, 5, 6, 10, 15, 25, 30, 50, 75, 150]$. All divisors except $75$ and $150$ are present in the $10 \times 10$ table. Array $a$ $=$ $[1, 1, 1, 1, 1, 1, 3, 5, 3, 5, 0, 0]$. There are $10$ non-zero values, and xor of $a$ is equal to $0$.</p><p>In the third test case, $m = 1 \cdot 210 = 210$ and has $16$ divisors $[1, 2, 3, 5, 6, 7, 10, 14, 15, 21, 30, 35, 42, 70, 105, 210]$. The $6 \times 6$ table with marked divisors is shown below:</p><center> <center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">1</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">6</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">2</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">3</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">5</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">6</span></td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">8</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">10</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">12</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">9</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">12</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">15</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">18</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">8</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">12</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">16</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">20</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">24</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">10</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">15</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">20</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">25</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">30</span></td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">12</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">18</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">24</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">30</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">36</td></tr></tbody></table> </center> </center><p>Array $a$ $=$ $[1, 1, 1, 1, 1, 0, 2, 0, 3, 0, 5, 0, 0, 0, 0, 0]$. There are $8$ non-zero values, and xor of $a$ is equal to $5$.</p>