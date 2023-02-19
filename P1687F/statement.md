## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">As she closed the Satori's eye that could read minds, Koishi gained the ability to live in unconsciousness. Even she herself does not know what she is up to.</span></div><div class="epigraph-source">— <span class="tex-font-style-it">Subterranean Animism</span></div></div><p>Koishi is unconsciously permuting $n$ numbers: $1, 2, \ldots, n$.</p><p>She thinks the permutation $p$ is <span class="tex-font-style-bf">beautiful</span> if $s=\sum\limits_{i=1}^{n-1} [p_i+1=p_{i+1}]$. $[x]$ equals to $1$ if $x$ holds, or $0$ otherwise.</p><p>For each $k\in[0,n-1]$, she wants to know the number of beautiful permutations of length $n$ satisfying $k=\sum\limits_{i=1}^{n-1}[p_i&lt;p_{i+1}]$.</p></div><div class="input-specification"><p>There is one line containing two intergers $n$ ($1 \leq n \leq 250\,000$) and $s$ ($0 \leq s &lt; n$).</p></div><div class="output-specification"><p>Print one line with $n$ intergers. The $i$-th integers represents the answer of $k=i-1$, modulo $998244353$.</p></div>

## Input

<p>There is one line containing two intergers $n$ ($1 \leq n \leq 250\,000$) and $s$ ($0 \leq s &lt; n$).</p>

## Output

<p>Print one line with $n$ intergers. The $i$-th integers represents the answer of $k=i-1$, modulo $998244353$.</p>





```input1
2 0
```




```input2
4 1
```




```input3
8 3
```




```output1
1 0
```




```output2
0 3 6 0
```




```output3
0 0 0 35 770 980 70 0
```



## Note

<p>Let $f(p)=\sum\limits_{i=1}^{n-1}[p_i&lt;p_{i+1}]$.</p><p>Testcase 1:</p><p>$[2,1]$ is the only beautiful permutation. And $f([2,1])=0$.</p><p>Testcase 2:</p><p>Beautiful permutations:</p><p>$[1,2,4,3]$, $[1,3,4,2]$, $[1,4,2,3]$, $[2,1,3,4]$, $[2,3,1,4]$, $[3,1,2,4]$, $[3,4,2,1]$, $[4,2,3,1]$, $[4,3,1,2]$. The first six of them satisfy $f(p)=2$, while others satisfy $f(p)=1$.</p>
