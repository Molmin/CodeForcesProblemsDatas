## Description

<div><p>You are given a sequence $A$, where its elements are either in the form <span class="tex-font-style-tt">+ x</span> or <span class="tex-font-style-tt">-</span>, where $x$ is an integer.</p><p>For such a sequence $S$ where its elements are either in the form <span class="tex-font-style-tt">+ x</span> or <span class="tex-font-style-tt">-</span>, define $f(S)$ as follows:</p><ul> <li> iterate through $S$'s elements from the first one to the last one, and maintain a multiset $T$ as you iterate through it. </li><li> for each element, if it's in the form <span class="tex-font-style-tt">+ x</span>, add $x$ to $T$; otherwise, erase the smallest element from $T$ (if $T$ is empty, do nothing). </li><li> after iterating through all $S$'s elements, compute the sum of all elements in $T$. $f(S)$ is defined as the sum. </li></ul><p>The sequence $b$ is a subsequence of the sequence $a$ if $b$ can be derived from $a$ by removing zero or more elements without changing the order of the remaining elements. For all $A$'s subsequences $B$, compute the sum of $f(B)$, modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1\leq n\leq 500$) — the length of $A$.</p><p>Each of the next $n$ lines begins with an operator <span class="tex-font-style-tt">+</span> or <span class="tex-font-style-tt">-</span>. If the operator is <span class="tex-font-style-tt">+</span>, then it's followed by an integer $x$ ($1\le x&lt;998\,244\,353$). The $i$-th line of those $n$ lines describes the $i$-th element in $A$.</p></div><div class="output-specification"><p>Print one integer, which is the answer to the problem, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1\leq n\leq 500$) — the length of $A$.</p><p>Each of the next $n$ lines begins with an operator <span class="tex-font-style-tt">+</span> or <span class="tex-font-style-tt">-</span>. If the operator is <span class="tex-font-style-tt">+</span>, then it's followed by an integer $x$ ($1\le x&lt;998\,244\,353$). The $i$-th line of those $n$ lines describes the $i$-th element in $A$.</p>

## Output

<p>Print one integer, which is the answer to the problem, modulo $998\,244\,353$.</p>





```input1
4
-
+ 1
+ 2
-
```




```input2
15
+ 2432543
-
+ 4567886
+ 65638788
-
+ 578943
-
-
+ 62356680
-
+ 711111
-
+ 998244352
-
-
```




```output1
16
```




```output2
750759115
```



## Note

<p>In the first example, the following are all possible pairs of $B$ and $f(B)$:</p><ul> <li> $B=$ <span class="tex-font-style-tt">{}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{-}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 1, -}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 1, -}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 2, -}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 2, -}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{-}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{-, -}</span>, $f(B)=0$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 1, + 2}</span>, $f(B)=3$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 1, + 2, -}</span>, $f(B)=2$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 1, + 2}</span>, $f(B)=3$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 1, + 2, -}</span>, $f(B)=2$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 1}</span>, $f(B)=1$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 1}</span>, $f(B)=1$. </li><li> $B=$ <span class="tex-font-style-tt">{-, + 2}</span>, $f(B)=2$. </li><li> $B=$ <span class="tex-font-style-tt">{+ 2}</span>, $f(B)=2$. </li></ul><p>The sum of these values is $16$.</p>
