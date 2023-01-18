## Description

<div><p>Bessie the cow has just intercepted a text that Farmer John sent to Burger Queen! However, Bessie is sure that there is a secret message hidden inside.</p><p>The text is a string $s$ of lowercase Latin letters. She considers a string $t$ as hidden in string $s$ if $t$ exists as a subsequence of $s$ whose indices form an arithmetic progression. For example, the string <span class="tex-font-style-tt">aab</span> is hidden in string <span class="tex-font-style-tt">aaabb</span> because it occurs at indices $1$, $3$, and $5$, which form an arithmetic progression with a common difference of $2$. Bessie thinks that any hidden string that occurs the most times is the secret message. Two occurrences of a subsequence of $S$ are distinct if the sets of indices are different. Help her find the number of occurrences of the secret message!</p><p>For example, in the string <span class="tex-font-style-tt">aaabb</span>, <span class="tex-font-style-tt">a</span> is hidden $3$ times, <span class="tex-font-style-tt">b</span> is hidden $2$ times, <span class="tex-font-style-tt">ab</span> is hidden $6$ times, <span class="tex-font-style-tt">aa</span> is hidden $3$ times, <span class="tex-font-style-tt">bb</span> is hidden $1$ time, <span class="tex-font-style-tt">aab</span> is hidden $2$ times, <span class="tex-font-style-tt">aaa</span> is hidden $1$ time, <span class="tex-font-style-tt">abb</span> is hidden $1$ time, <span class="tex-font-style-tt">aaab</span> is hidden $1$ time, <span class="tex-font-style-tt">aabb</span> is hidden $1$ time, and <span class="tex-font-style-tt">aaabb</span> is hidden $1$ time. The number of occurrences of the secret message is $6$.</p></div><div class="input-specification"><p>The first line contains a string $s$ of lowercase Latin letters ($1 \le |s| \le 10^5$) — the text that Bessie intercepted.</p></div><div class="output-specification"><p>Output a single integer &nbsp;— the number of occurrences of the secret message.</p></div>

## Input

<p>The first line contains a string $s$ of lowercase Latin letters ($1 \le |s| \le 10^5$) — the text that Bessie intercepted.</p>

## Output

<p>Output a single integer &nbsp;— the number of occurrences of the secret message.</p>





```input1
aaabb
```




```input2
usaco
```




```input3
lol
```




```output1
6
```




```output2
1
```




```output3
2
```



## Note

<p>In the first example, these are all the hidden strings and their indice sets: </p><ul> <li> <span class="tex-font-style-tt">a</span> occurs at $(1)$, $(2)$, $(3)$ </li><li> <span class="tex-font-style-tt">b</span> occurs at $(4)$, $(5)$ </li><li> <span class="tex-font-style-tt">ab</span> occurs at $(1,4)$, $(1,5)$, $(2,4)$, $(2,5)$, $(3,4)$, $(3,5)$ </li><li> <span class="tex-font-style-tt">aa</span> occurs at $(1,2)$, $(1,3)$, $(2,3)$ </li><li> <span class="tex-font-style-tt">bb</span> occurs at $(4,5)$ </li><li> <span class="tex-font-style-tt">aab</span> occurs at $(1,3,5)$, $(2,3,4)$ </li><li> <span class="tex-font-style-tt">aaa</span> occurs at $(1,2,3)$ </li><li> <span class="tex-font-style-tt">abb</span> occurs at $(3,4,5)$ </li><li> <span class="tex-font-style-tt">aaab</span> occurs at $(1,2,3,4)$ </li><li> <span class="tex-font-style-tt">aabb</span> occurs at $(2,3,4,5)$ </li><li> <span class="tex-font-style-tt">aaabb</span> occurs at $(1,2,3,4,5)$ </li></ul> Note that all the sets of indices are arithmetic progressions.<p>In the second example, no hidden string occurs more than once.</p><p>In the third example, the hidden string is the letter <span class="tex-font-style-tt">l</span>.</p>
