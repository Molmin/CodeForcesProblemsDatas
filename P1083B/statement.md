## Description

<div><p>Recently, the Fair Nut has written $k$ strings of length $n$, consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". He calculated $c$&nbsp;— the number of strings that are prefixes of at least one of the written strings. <span class="tex-font-style-bf">Every string was counted only one time</span>.</p><p>Then, he lost his sheet with strings. He remembers that all written strings were lexicographically <span class="tex-font-style-bf">not smaller</span> than string $s$ and <span class="tex-font-style-bf">not bigger</span> than string $t$. He is interested: what is the maximum value of $c$ that he could get.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$.</li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 5 \cdot 10^5$, $1 \leq k \leq 10^9$).</p><p>The second line contains a string $s$ ($|s| = n$)&nbsp;— the string consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>.</p><p>The third line contains a string $t$ ($|t| = n$)&nbsp;— the string consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>.</p><p>It is guaranteed that string $s$ is lexicographically not bigger than $t$.</p></div><div class="output-specification"><p>Print one number&nbsp;— maximal value of $c$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq n \leq 5 \cdot 10^5$, $1 \leq k \leq 10^9$).</p><p>The second line contains a string $s$ ($|s| = n$)&nbsp;— the string consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>.</p><p>The third line contains a string $t$ ($|t| = n$)&nbsp;— the string consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>.</p><p>It is guaranteed that string $s$ is lexicographically not bigger than $t$.</p>

## Output

<p>Print one number&nbsp;— maximal value of $c$.</p>





```input1
2 4
aa
bb
```




```input2
3 3
aba
bba
```




```input3
4 5
abbb
baaa
```




```output1
6
```




```output2
8
```




```output3
8
```



## Note

<p>In the first example, Nut could write strings "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">bb</span>". These $4$ strings are prefixes of at least one of the written strings, as well as "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". Totally, $6$ strings.</p><p>In the second example, Nut could write strings "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">baa</span>", "<span class="tex-font-style-tt">bba</span>".</p><p>In the third example, there are only two different strings that Nut could write. If both of them are written, $c=8$.</p>
