## Description

<div><p>Toad Rash has a binary string $s$. A binary string consists only of zeros and ones.</p><p>Let $n$ be the length of $s$.</p><p>Rash needs to find the number of such pairs of integers $l$, $r$ that $1 \leq l \leq r \leq n$ and there is at least one pair of integers $x$, $k$ such that $1 \leq x, k \leq n$, $l \leq x &lt; x + 2k \leq r$, and $s_x = s_{x+k} = s_{x+2k}$.</p><p>Find this number of pairs for Rash.</p></div><div class="input-specification"><p>The first line contains the string $s$ ($1 \leq |s| \leq 300\,000$), consisting of zeros and ones.</p></div><div class="output-specification"><p>Output one integer: the number of such pairs of integers $l$, $r$ that $1 \leq l \leq r \leq n$ and there is at least one pair of integers $x$, $k$ such that $1 \leq x, k \leq n$, $l \leq x &lt; x + 2k \leq r$, and $s_x = s_{x+k} = s_{x+2k}$.</p></div>

## Input

<p>The first line contains the string $s$ ($1 \leq |s| \leq 300\,000$), consisting of zeros and ones.</p>

## Output

<p>Output one integer: the number of such pairs of integers $l$, $r$ that $1 \leq l \leq r \leq n$ and there is at least one pair of integers $x$, $k$ such that $1 \leq x, k \leq n$, $l \leq x &lt; x + 2k \leq r$, and $s_x = s_{x+k} = s_{x+2k}$.</p>





```input1
010101
```




```input2
11001100
```




```output1
3
```




```output2
0
```



## Note

<p>In the first example, there are three $l$, $r$ pairs we need to count: $1$, $6$; $2$, $6$; and $1$, $5$.</p><p>In the second example, there are no values $x$, $k$ for the initial string, so the answer is $0$.</p>
