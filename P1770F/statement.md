## Description

<div><p>Mari has three integers $n$, $x$, and $y$.</p><p>Call an array $a$ of $n$ <span class="tex-font-style-bf">non-negative</span> integers <span class="tex-font-style-it">good</span> if it satisfies the following conditions:</p><ul> <li> $a_1+a_2+\ldots+a_n=x$, and </li><li> $a_1 \, | \, a_2 \, | \, \ldots \, | \, a_n=y$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. </li></ul><p>The <span class="tex-font-style-it">score</span> of a good array is the value of $a_1 \oplus a_2 \oplus \ldots \oplus a_n$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Koxia wants you to find the total bitwise XOR of the scores of all good arrays. If there are no good arrays, output $0$ instead.</p></div><div class="input-specification"><p>The first line of input contains three integers $n$, $x$ and $y$ ($1 \leq n &lt; 2^{40}$, $0 \leq x &lt; 2^{60}$, $0 \leq y &lt; 2^{20}$).</p></div><div class="output-specification"><p>Output a single integer — the total bitwise XOR of the scores of all good arrays.</p></div>

## Input

<p>The first line of input contains three integers $n$, $x$ and $y$ ($1 \leq n &lt; 2^{40}$, $0 \leq x &lt; 2^{60}$, $0 \leq y &lt; 2^{20}$).</p>

## Output

<p>Output a single integer — the total bitwise XOR of the scores of all good arrays.</p>





```input1
3 5 3
```




```input2
100 0 100
```




```input3
79877974817 749875791743978 982783
```




```output1
2
```




```output2
0
```




```output3
64
```



## Note

<p>In the first test case, there are $12$ good arrays totally as follows.</p><ul> <li> $[0,2,3]$, $[0,3,2]$, $[2,0,3]$, $[2,3,0]$, $[3,0,2]$ and $[3,2,0]$ — the score is $0 \oplus 2 \oplus 3 = 1$; </li><li> $[1, 2, 2]$, $[2, 1, 2]$ and $[2, 2, 1]$ — the score is $1 \oplus 2 \oplus 2 = 1$; </li><li> $[1, 1, 3]$, $[1, 3, 1]$ and $[3, 1, 1]$ — the score is $1 \oplus 1 \oplus 3 = 3$. </li></ul><p>Therefore, the total bitwise xor of the scores is $\underbrace{1 \oplus \ldots \oplus 1}_{9\text{ times}} \oplus 3 \oplus 3 \oplus 3 = 2$.</p><p>In the second test case, there are no good sequences. The output should be $0$.</p>
