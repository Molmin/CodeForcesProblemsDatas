## Description

<div><p>You are given two strings of equal length $s$ and $t$ consisting of lowercase Latin letters. You may perform any number (possibly, zero) operations on these strings.</p><p>During each operation you choose two <span class="tex-font-style-bf">adjacent</span> characters in <span class="tex-font-style-bf">any</span> string and assign the value of the first character to the value of the second or vice versa.</p><p>For example, if $s$ is "<span class="tex-font-style-tt">acbc</span>" you can get the following strings in <span class="tex-font-style-bf">one</span> operation: </p><ul> <li> "<span class="tex-font-style-tt">aabc</span>" (if you perform $s_2 = s_1$); </li><li> "<span class="tex-font-style-tt">ccbc</span>" (if you perform $s_1 = s_2$); </li><li> "<span class="tex-font-style-tt">accc</span>" (if you perform $s_3 = s_2$ or $s_3 = s_4$); </li><li> "<span class="tex-font-style-tt">abbc</span>" (if you perform $s_2 = s_3$); </li><li> "<span class="tex-font-style-tt">acbb</span>" (if you perform $s_4 = s_3$); </li></ul><p>Note that you can also apply this operation to the string $t$.</p><p>Please determine whether it is possible to transform $s$ into $t$, applying the operation above any number of times.</p><p>Note that you have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 100$)&nbsp;— the number of queries. Each query is represented by two consecutive lines.</p><p>The first line of each query contains the string $s$ ($1 \le |s| \le 100$) consisting of lowercase Latin letters.</p><p>The second line of each query contains the string $t$ ($1 \le |t| \leq 100$, $|t| = |s|$) consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each query, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make $s$ equal to $t$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 100$)&nbsp;— the number of queries. Each query is represented by two consecutive lines.</p><p>The first line of each query contains the string $s$ ($1 \le |s| \le 100$) consisting of lowercase Latin letters.</p><p>The second line of each query contains the string $t$ ($1 \le |t| \leq 100$, $|t| = |s|$) consisting of lowercase Latin letters.</p>

## Output

<p>For each query, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make $s$ equal to $t$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will all be recognized as positive answer).</p>





```input1
3
xabb
aabx
technocup
technocup
a
z
```




```output1
YES
YES
NO
```



## Note

<p>In the first query, you can perform two operations $s_1 = s_2$ (after it $s$ turns into "<span class="tex-font-style-tt">aabb</span>") and $t_4 = t_3$ (after it $t$ turns into "<span class="tex-font-style-tt">aabb</span>"). </p><p>In the second query, the strings are equal initially, so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the third query, you can not make strings $s$ and $t$ equal. Therefore, the answer is "<span class="tex-font-style-tt">NO</span>".</p>
