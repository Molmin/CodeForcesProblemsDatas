## Description

<div><p>Let's name a pair of positive integers $(x, y)$ <span class="tex-font-style-it">lucky</span> if the greatest common divisor of them is equal to $1$ ($\gcd(x, y) = 1$).</p><p>Let's define a <span class="tex-font-style-it">chain</span> induced by $(x, y)$ as a sequence of pairs $(x, y)$, $(x + 1, y + 1)$, $(x + 2, y + 2)$, $\dots$, $(x + k, y + k)$ for some integer $k \ge 0$. The <span class="tex-font-style-it">length</span> of the chain is the number of pairs it consists of, or $(k + 1)$.</p><p>Let's name such chain <span class="tex-font-style-it">lucky</span> if all pairs in the chain are lucky.</p><p>You are given $n$ pairs $(x_i, y_i)$. Calculate for each pair the length of the longest lucky chain induced by this pair. Note that if $(x_i, y_i)$ is not lucky itself, the chain will have the length $0$. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of pairs.</p><p>Next $n$ lines contains $n$ pairs&nbsp;— one per line. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i &lt; y_i \le 10^7$)&nbsp;— the corresponding pair.</p></div><div class="output-specification"><p>Print $n$ integers, where the $i$-th integer is the length of the longest lucky chain induced by $(x_i, y_i)$ or $-1$ if the chain can be infinitely long.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of pairs.</p><p>Next $n$ lines contains $n$ pairs&nbsp;— one per line. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i &lt; y_i \le 10^7$)&nbsp;— the corresponding pair.</p>

## Output

<p>Print $n$ integers, where the $i$-th integer is the length of the longest lucky chain induced by $(x_i, y_i)$ or $-1$ if the chain can be infinitely long.</p>





```input1
4
5 15
13 37
8 9
10009 20000
```




```output1
0
1
-1
79
```



## Note

<p>In the first test case, $\gcd(5, 15) = 5 &gt; 1$, so it's already not lucky, so the length of the lucky chain is $0$.</p><p>In the second test case, $\gcd(13 + 1, 37 + 1) = \gcd(14, 38) = 2$. So, the lucky chain consists of the single pair $(13, 37)$. </p>
