## Description

<div><p>Given a string $s$ of length $n$ and integer $k$ ($1 \le k \le n$). The string $s$ has a level $x$, if $x$ is largest non-negative integer, such that it's possible to find in $s$:</p><ul> <li> $x$ <span class="tex-font-style-bf">non-intersecting</span> (non-overlapping) substrings of length $k$, </li><li> all characters of these $x$ substrings are the same (i.e. each substring contains only one distinct character and this character is the same for all the substrings). </li></ul><p>A substring is a sequence of consecutive (adjacent) characters, it is defined by two integers $i$ and $j$ ($1 \le i \le j \le n$), denoted as $s[i \dots j]$ = "$s_{i}s_{i+1} \dots s_{j}$".</p><p>For example, if $k = 2$, then:</p><ul> <li> the string "<span class="tex-font-style-tt">aabb</span>" has level $1$ (you can select substring "<span class="tex-font-style-tt">aa</span>"), </li><li> the strings "<span class="tex-font-style-tt">zzzz</span>" and "<span class="tex-font-style-tt">zzbzz</span>" has level $2$ (you can select two non-intersecting substrings "<span class="tex-font-style-tt">zz</span>" in each of them), </li><li> the strings "<span class="tex-font-style-tt">abed</span>" and "<span class="tex-font-style-tt">aca</span>" have level $0$ (you can't find at least one substring of the length $k=2$ containing the only distinct character). </li></ul><p>Zuhair gave you the integer $k$ and the string $s$ of length $n$. You need to find $x$, the level of the string $s$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string and the value of $k$.</p><p>The second line contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p></div><div class="output-specification"><p>Print a single integer $x$&nbsp;— the level of the string.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string and the value of $k$.</p><p>The second line contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p>

## Output

<p>Print a single integer $x$&nbsp;— the level of the string.</p>





```input1
8 2
aaacaabb
```




```input2
2 1
ab
```




```input3
4 2
abab
```




```output1
2
```




```output2
1
```




```output3
0
```



## Note

<p>In the first example, we can select $2$ non-intersecting substrings consisting of letter '<span class="tex-font-style-tt">a</span>': "<span class="tex-font-style-tt">(aa)ac(aa)bb</span>", so the level is $2$.</p><p>In the second example, we can select either substring "<span class="tex-font-style-tt">a</span>" or "<span class="tex-font-style-tt">b</span>" to get the answer $1$.</p>
