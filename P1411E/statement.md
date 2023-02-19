## Description

<div><p>You've got a string $S$ consisting of $n$ lowercase English letters from your friend. It turned out that this is a number written in <span class="tex-font-style-it">poman</span> numerals. The poman numeral system is long forgotten. All that's left is the algorithm to transform number from poman numerals to the numeral system familiar to us. Characters of $S$ are numbered from $1$ to $n$ from left to right. Let's denote the value of $S$ as $f(S)$, it is defined as follows: </p><ul> <li> If $|S| &gt; 1$, an arbitrary integer $m$ ($1 \le m &lt; |S|$) is chosen, and it is defined that $f(S) = -f(S[1, m]) + f(S[m + 1, |S|])$, where $S[l, r]$ denotes the substring of $S$ from the $l$-th to the $r$-th position, inclusively. </li><li> Otherwise $S = c$, where $c$ is some English letter. Then $f(S) = 2^{pos(c)}$, where $pos(c)$ is the position of letter $c$ in the alphabet ($pos($<span class="tex-font-style-tt">a</span>$) = 0$, $pos($<span class="tex-font-style-tt">z</span>$) = 25$). </li></ul><p>Note that $m$ is chosen independently on each step.</p><p>Your friend thinks it is possible to get $f(S) = T$ by choosing the right $m$ on every step. Is he right?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $T$ ($2 \leq n \leq 10^5$, $-10^{15} \leq T \leq 10^{15}$).</p><p>The second line contains a string $S$ consisting of $n$ lowercase English letters.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if it is possible to get the desired value. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $n$ and $T$ ($2 \leq n \leq 10^5$, $-10^{15} \leq T \leq 10^{15}$).</p><p>The second line contains a string $S$ consisting of $n$ lowercase English letters.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if it is possible to get the desired value. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
2 -1
ba
```




```input2
3 -7
abc
```




```input3
7 -475391
qohshra
```




```output1
Yes
```




```output2
No
```




```output3
Yes
```



## Note

<p>In the second example, you cannot get $-7$. But you can get $1$, for example, as follows: </p><ol> <li> First choose $m = 1$, then $f($<span class="tex-font-style-tt">abc</span>$) = -f($<span class="tex-font-style-tt">a</span>$) + f($<span class="tex-font-style-tt">bc</span>$)$ </li><li> $f($<span class="tex-font-style-tt">a</span>$) = 2^0 = 1$ </li><li> $f($<span class="tex-font-style-tt">bc</span>$) = -f($<span class="tex-font-style-tt">b</span>$) + f($<span class="tex-font-style-tt">c</span>$) = -2^1 + 2^2 = 2$ </li><li> In the end $f($<span class="tex-font-style-tt">abc</span>$) = -1 + 2 = 1$ </li></ol>
