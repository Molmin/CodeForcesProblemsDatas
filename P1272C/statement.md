## Description

<div><p>Recently, Norge found a string $s = s_1 s_2 \ldots s_n$ consisting of $n$ lowercase Latin letters. As an exercise to improve his typing speed, he decided to type all substrings of the string $s$. Yes, all $\frac{n (n + 1)}{2}$ of them!</p><p>A substring of $s$ is a non-empty string $x = s[a \ldots b] = s_{a} s_{a + 1} \ldots s_{b}$ ($1 \leq a \leq b \leq n$). For example, "<span class="tex-font-style-tt">auto</span>" and "<span class="tex-font-style-tt">ton</span>" are substrings of "<span class="tex-font-style-tt">automaton</span>".</p><p>Shortly after the start of the exercise, Norge realized that his keyboard was broken, namely, he could use only $k$ Latin letters $c_1, c_2, \ldots, c_k$ out of $26$.</p><p>After that, Norge became interested in how many substrings of the string $s$ he could still type using his broken keyboard. Help him to find this number.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 26$) — the length of the string $s$ and the number of Latin letters still available on the keyboard.</p><p>The second line contains the string $s$ consisting of exactly $n$ lowercase Latin letters.</p><p>The third line contains $k$ space-separated distinct lowercase Latin letters $c_1, c_2, \ldots, c_k$ — the letters still available on the keyboard.</p></div><div class="output-specification"><p>Print a single number — the number of substrings of $s$ that can be typed using only available letters $c_1, c_2, \ldots, c_k$.</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq 26$) — the length of the string $s$ and the number of Latin letters still available on the keyboard.</p><p>The second line contains the string $s$ consisting of exactly $n$ lowercase Latin letters.</p><p>The third line contains $k$ space-separated distinct lowercase Latin letters $c_1, c_2, \ldots, c_k$ — the letters still available on the keyboard.</p>

## Output

<p>Print a single number — the number of substrings of $s$ that can be typed using only available letters $c_1, c_2, \ldots, c_k$.</p>





```input1
7 2
abacaba
a b
```




```input2
10 3
sadfaasdda
f a d
```




```input3
7 1
aaaaaaa
b
```




```output1
12
```




```output2
21
```




```output3
0
```



## Note

<p>In the first example Norge can print substrings $s[1\ldots2]$, $s[2\ldots3]$, $s[1\ldots3]$, $s[1\ldots1]$, $s[2\ldots2]$, $s[3\ldots3]$, $s[5\ldots6]$, $s[6\ldots7]$, $s[5\ldots7]$, $s[5\ldots5]$, $s[6\ldots6]$, $s[7\ldots7]$.</p>
