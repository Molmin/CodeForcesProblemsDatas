## Description

<div><p>You are given three strings $s$, $t$ and $p$ consisting of lowercase Latin letters. You may perform any number (possibly, zero) operations on these strings.</p><p>During each operation you choose any character from $p$, erase it from $p$ and insert it into string $s$ (you may insert this character anywhere you want: in the beginning of $s$, in the end or between any two consecutive characters). </p><p>For example, if $p$ is <span class="tex-font-style-tt">aba</span>, and $s$ is <span class="tex-font-style-tt">de</span>, then the following outcomes are possible (the character we erase from $p$ and insert into $s$ is highlighted):</p><ul> <li> <span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">ba</span> $\rightarrow$ <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">de</span>; </li><li> <span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">ba</span> $\rightarrow$ <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">d</span><span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">e</span>; </li><li> <span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">ba</span> $\rightarrow$ <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">de</span><span class="tex-font-style-bf">a</span>; </li><li> <span class="tex-font-style-tt">a</span><span class="tex-font-style-bf">b</span><span class="tex-font-style-tt">a</span> $\rightarrow$ <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-bf">b</span><span class="tex-font-style-tt">de</span>; </li><li> <span class="tex-font-style-tt">a</span><span class="tex-font-style-bf">b</span><span class="tex-font-style-tt">a</span> $\rightarrow$ <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">d</span><span class="tex-font-style-bf">b</span><span class="tex-font-style-tt">e</span>; </li><li> <span class="tex-font-style-tt">a</span><span class="tex-font-style-bf">b</span><span class="tex-font-style-tt">a</span> $\rightarrow$ <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">de</span><span class="tex-font-style-bf">b</span>; </li><li> <span class="tex-font-style-tt">ab</span><span class="tex-font-style-bf">a</span> $\rightarrow$ <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">de</span>; </li><li> <span class="tex-font-style-tt">ab</span><span class="tex-font-style-bf">a</span> $\rightarrow$ <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">d</span><span class="tex-font-style-bf">a</span><span class="tex-font-style-tt">e</span>; </li><li> <span class="tex-font-style-tt">ab</span><span class="tex-font-style-bf">a</span> $\rightarrow$ <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">de</span> $\rightarrow$ <span class="tex-font-style-tt">de</span><span class="tex-font-style-bf">a</span>; </li></ul><p>Your goal is to perform several (maybe zero) operations so that $s$ becomes equal to $t$. Please determine whether it is possible.</p><p>Note that you have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 100$) — the number of queries. Each query is represented by three consecutive lines.</p><p>The first line of each query contains the string $s$ ($1 \le |s| \le 100$) consisting of lowercase Latin letters.</p><p>The second line of each query contains the string $t$ ($1 \le |t| \le 100$) consisting of lowercase Latin letters.</p><p>The third line of each query contains the string $p$ ($1 \le |p| \le 100$) consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each query print <span class="tex-font-style-tt">YES</span> if it is possible to make $s$ equal to $t$, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 100$) — the number of queries. Each query is represented by three consecutive lines.</p><p>The first line of each query contains the string $s$ ($1 \le |s| \le 100$) consisting of lowercase Latin letters.</p><p>The second line of each query contains the string $t$ ($1 \le |t| \le 100$) consisting of lowercase Latin letters.</p><p>The third line of each query contains the string $p$ ($1 \le |p| \le 100$) consisting of lowercase Latin letters.</p>

## Output

<p>For each query print <span class="tex-font-style-tt">YES</span> if it is possible to make $s$ equal to $t$, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
4
ab
acxb
cax
a
aaaa
aaabbcc
a
aaaa
aabbcc
ab
baaa
aaaaa
```




```output1
YES
YES
NO
NO
```



## Note

<p>In the first test case there is the following sequence of operation: </p><ol> <li> $s = $ <span class="tex-font-style-tt">ab</span>, $t = $ <span class="tex-font-style-tt">acxb</span>, $p = $ <span class="tex-font-style-tt">cax</span>; </li><li> $s = $ <span class="tex-font-style-tt">acb</span>, $t = $ <span class="tex-font-style-tt">acxb</span>, $p = $ <span class="tex-font-style-tt">ax</span>; </li><li> $s = $ <span class="tex-font-style-tt">acxb</span>, $t = $ <span class="tex-font-style-tt">acxb</span>, $p = $ <span class="tex-font-style-tt">a</span>. </li></ol><p>In the second test case there is the following sequence of operation: </p><ol> <li> $s = $ <span class="tex-font-style-tt">a</span>, $t = $ <span class="tex-font-style-tt">aaaa</span>, $p = $ <span class="tex-font-style-tt">aaabbcc</span>; </li><li> $s = $ <span class="tex-font-style-tt">aa</span>, $t = $ <span class="tex-font-style-tt">aaaa</span>, $p = $ <span class="tex-font-style-tt">aabbcc</span>; </li><li> $s = $ <span class="tex-font-style-tt">aaa</span>, $t = $ <span class="tex-font-style-tt">aaaa</span>, $p = $ <span class="tex-font-style-tt">abbcc</span>; </li><li> $s = $ <span class="tex-font-style-tt">aaaa</span>, $t = $ <span class="tex-font-style-tt">aaaa</span>, $p = $ <span class="tex-font-style-tt">bbcc</span>. </li></ol>
