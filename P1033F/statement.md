## Description

<div><p>Alice has a computer that operates on $w$-bit integers. The computer has $n$ <span class="tex-font-style-bf">registers</span> for values. The current content of the registers is given as an array $a_1, a_2, \ldots, a_n$. </p><p>The computer uses so-called "<span class="tex-font-style-it">number gates</span>" to manipulate this data. Each "<span class="tex-font-style-it">number gate</span>" takes two registers as inputs and calculates a function of the two values stored in those registers. Note that you can use the same register as both inputs.</p><p>Each "<span class="tex-font-style-it">number gate</span>" is assembled from bit gates. There are six types of bit gates: <span class="tex-font-style-tt">AND</span>, <span class="tex-font-style-tt">OR</span>, <span class="tex-font-style-tt">XOR</span>, <span class="tex-font-style-tt">NOT&nbsp;AND</span>, <span class="tex-font-style-tt">NOT&nbsp;OR</span>, and <span class="tex-font-style-tt">NOT&nbsp;XOR</span>, denoted "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">O</span>", "<span class="tex-font-style-tt">X</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">x</span>", respectively. Each <span class="tex-font-style-bf">bit gate</span> takes two bits as input. Its output given the input bits $b_1$, $b_2$ is given below:</p><center> $\begin{matrix} b_1 &amp; b_2 &amp; A &amp; O &amp; X &amp; a &amp; o &amp; x \\ 0 &amp; 0 &amp; 0 &amp; 0 &amp; 0 &amp; 1 &amp; 1 &amp; 1 \\ 0 &amp; 1 &amp; 0 &amp; 1 &amp; 1 &amp; 1 &amp; 0 &amp; 0 \\ 1 &amp; 0 &amp; 0 &amp; 1 &amp; 1 &amp; 1 &amp; 0 &amp; 0 \\ 1 &amp; 1 &amp; 1 &amp; 1 &amp; 0 &amp; 0 &amp; 0 &amp; 1 \\ \end{matrix}$ </center><p>To build a "<span class="tex-font-style-it">number gate</span>", one takes $w$ bit gates and assembles them into an array. A "<span class="tex-font-style-it">number gate</span>" takes two $w$-bit integers $x_1$ and $x_2$ as input. The "<span class="tex-font-style-it">number gate</span>" splits the integers into $w$ bits and feeds the $i$-th bit of each input to the $i$-th bit gate. After that, it assembles the resulting bits again to form an output word. </p><p>For instance, for $4$-bit computer we might have a "<span class="tex-font-style-it">number gate</span>" "<span class="tex-font-style-tt">AXoA</span>" (<span class="tex-font-style-tt">AND</span>, <span class="tex-font-style-tt">XOR</span>, <span class="tex-font-style-tt">NOT OR</span>, <span class="tex-font-style-tt">AND</span>). For two inputs, $13 = 1101_2$ and $10 = 1010_2$, this returns $12 = 1100_2$, as $1$ <span class="tex-font-style-tt">and</span> $1$ is $1$, $1$ <span class="tex-font-style-tt">xor</span> $0$ is $1$, <span class="tex-font-style-tt">not</span> ($0$ <span class="tex-font-style-tt">or</span> $1$) is $0$, and finally $1$ <span class="tex-font-style-tt">and</span> $0$ is $0$. </p><p>You are given a description of $m$ "<span class="tex-font-style-it">number gates</span>". For each gate, your goal is to report the number of register pairs for which the "<span class="tex-font-style-it">number gate</span>" outputs the number $0$. In other words, find the number of ordered pairs $(i,j)$ where $1 \leq i,j \leq n$, such that $w_k(a_i, a_j) = 0$, where $w_k$ is the function computed by the $k$-th "<span class="tex-font-style-it">number gate</span>".</p></div><div class="input-specification"><p>The first line contains three integers: $w$, $n$, and $m~(1 \leq w \leq 12, 1 \leq n \leq 3\cdot 10^4, 1 \leq m \leq 5\cdot 10^4)$&nbsp;— the word size, the number of variables, and the number of gates.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(0 \leq a_i &lt; 2^w)$&nbsp;— the value of variables stored in the registers.</p><p>Each of the next $m$ lines contains a string $g_j~(|g_j| = w)$ with a description of a single gate. Each character of $g_j$ is one of "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">O</span>", "<span class="tex-font-style-tt">X</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">x</span>".</p></div><div class="output-specification"><p>Print $m$ lines. The $i$-th line should contain the number of ordered pairs of variables for which the $i$-th gate returns zero.</p></div>

## Input

<p>The first line contains three integers: $w$, $n$, and $m~(1 \leq w \leq 12, 1 \leq n \leq 3\cdot 10^4, 1 \leq m \leq 5\cdot 10^4)$&nbsp;— the word size, the number of variables, and the number of gates.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(0 \leq a_i &lt; 2^w)$&nbsp;— the value of variables stored in the registers.</p><p>Each of the next $m$ lines contains a string $g_j~(|g_j| = w)$ with a description of a single gate. Each character of $g_j$ is one of "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">O</span>", "<span class="tex-font-style-tt">X</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">x</span>".</p>

## Output

<p>Print $m$ lines. The $i$-th line should contain the number of ordered pairs of variables for which the $i$-th gate returns zero.</p>





```input1
4 3 1
13 10 6
AXoA

```




```input2
1 7 6
0 1 1 0 1 0 0
A
O
X
a
o
x

```




```input3
6 2 4
47 12
AOXaox
AAaaAA
xxxxxx
XXXXXX

```




```input4
2 2 2
2 0
xO
Ox

```




```output1
3

```




```output2
40
16
25
9
33
24

```




```output3
2
3
0
2

```




```output4
2
0

```



## Note

<p>In the first test case, the inputs in binary are $1101$, $1010$, $0110$. The pairs that return $0$ are $(13, 6)$, $(6, 13)$, and $(6, 6)$. As it was already mentioned in the problem statement, $13 \oplus 10 = 10 \oplus 13 = 12$. The other pairs are $13 \oplus 13 = 11$, $10 \oplus 10 = 8$ and $10 \oplus 6 = 6 \oplus 10 = 4$. </p>
