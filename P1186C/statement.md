## Description

<div><p>Vus the Cossack has two binary strings, that is, strings that consist only of "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". We call these strings $a$ and $b$. It is known that $|b| \leq |a|$, that is, the length of $b$ is at most the length of $a$.</p><p>The Cossack considers every substring of length $|b|$ in string $a$. Let's call this substring $c$. He matches the corresponding characters in $b$ and $c$, after which he counts the number of positions where the two strings are different. We call this function $f(b, c)$.</p><p>For example, let $b = 00110$, and $c = 11000$. In these strings, the first, second, third and fourth positions are different.</p><p>Vus the Cossack counts the number of such substrings $c$ such that $f(b, c)$ is <span class="tex-font-style-bf">even</span>.</p><p>For example, let $a = 01100010$ and $b = 00110$. $a$ has four substrings of the length $|b|$: $01100$, $11000$, $10001$, $00010$. </p><ul><li> $f(00110, 01100) = 2$;</li><li> $f(00110, 11000) = 4$;</li><li> $f(00110, 10001) = 4$;</li><li> $f(00110, 00010) = 1$.</li></ul> <p>Since in three substrings, $f(b, c)$ is even, the answer is $3$.</p><p>Vus can not find the answer for big strings. That is why he is asking you to help him.</p></div><div class="input-specification"><p>The first line contains a binary string $a$ ($1 \leq |a| \leq 10^6$)&nbsp;— the first string.</p><p>The second line contains a binary string $b$ ($1 \leq |b| \leq |a|$)&nbsp;— the second string.</p></div><div class="output-specification"><p>Print one number&nbsp;— the answer.</p></div>

## Input

<p>The first line contains a binary string $a$ ($1 \leq |a| \leq 10^6$)&nbsp;— the first string.</p><p>The second line contains a binary string $b$ ($1 \leq |b| \leq |a|$)&nbsp;— the second string.</p>

## Output

<p>Print one number&nbsp;— the answer.</p>





```input1
01100010
00110
```




```input2
1010111110
0110
```




```output1
3
```




```output2
4
```



## Note

<p>The first example is explained in the legend.</p><p>In the second example, there are five substrings that satisfy us: $1010$, $0101$, $1111$, $1111$.</p>
