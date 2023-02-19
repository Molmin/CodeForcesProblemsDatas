## Description

<div><p>Your classmate, whom you do not like because he is boring, but whom you respect for his intellect, has two strings: $s$ of length $n$ and $t$ of length $m$.</p><p>A sequence $p_1, p_2, \ldots, p_m$, where $1 \leq p_1 &lt; p_2 &lt; \ldots &lt; p_m \leq n$, is called <span class="tex-font-style-it">beautiful</span>, if $s_{p_i} = t_i$ for all $i$ from $1$ to $m$. The <span class="tex-font-style-it">width</span> of a sequence is defined as $\max\limits_{1 \le i &lt; m} \left(p_{i + 1} - p_i\right)$.</p><p>Please help your classmate to identify the beautiful sequence with the <span class="tex-font-style-bf">maximum width</span>. Your classmate promised you that for the given strings $s$ and $t$ there is at least one beautiful sequence.</p></div><div class="input-specification"><p>The first input line contains two integers $n$ and $m$ ($2 \leq m \leq n \leq 2 \cdot 10^5$)&nbsp;— the lengths of the strings $s$ and $t$.</p><p>The following line contains a single string $s$ of length $n$, consisting of lowercase letters of the Latin alphabet.</p><p>The last line contains a single string $t$ of length $m$, consisting of lowercase letters of the Latin alphabet.</p><p>It is guaranteed that there is at least one beautiful sequence for the given strings.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum width of a beautiful sequence.</p></div>

## Input

<p>The first input line contains two integers $n$ and $m$ ($2 \leq m \leq n \leq 2 \cdot 10^5$)&nbsp;— the lengths of the strings $s$ and $t$.</p><p>The following line contains a single string $s$ of length $n$, consisting of lowercase letters of the Latin alphabet.</p><p>The last line contains a single string $t$ of length $m$, consisting of lowercase letters of the Latin alphabet.</p><p>It is guaranteed that there is at least one beautiful sequence for the given strings.</p>

## Output

<p>Output one integer&nbsp;— the maximum width of a beautiful sequence.</p>





```input1
5 3
abbbc
abc
```




```input2
5 2
aaaaa
aa
```




```input3
5 5
abcdf
abcdf
```




```input4
2 2
ab
ab
```




```output1
3
```




```output2
4
```




```output3
1
```




```output4
1
```



## Note

<p>In the first example there are two beautiful sequences of width $3$: they are $\{1, 2, 5\}$ and $\{1, 4, 5\}$.</p><p>In the second example the beautiful sequence with the maximum width is $\{1, 5\}$.</p><p>In the third example there is exactly one beautiful sequence&nbsp;— it is $\{1, 2, 3, 4, 5\}$.</p><p>In the fourth example there is exactly one beautiful sequence&nbsp;— it is $\{1, 2\}$.</p>
