## Description

<div><p>You are given a string $s$, consisting only of characters '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'. Let $|s|$ be the length of $s$.</p><p>You are asked to choose some integer $k$ ($k &gt; 0$) and find a sequence $a$ of length $k$ such that: </p><ul> <li> $1 \le a_1 &lt; a_2 &lt; \dots &lt; a_k \le |s|$; </li><li> $a_{i-1} + 1 &lt; a_i$ for all $i$ from $2$ to $k$. </li></ul><p>The characters at positions $a_1, a_2, \dots, a_k$ are removed, the remaining characters are concatenated without changing the order. So, in other words, the positions in the sequence $a$ should not be adjacent.</p><p>Let the resulting string be $s'$. $s'$ is called sorted if for all $i$ from $2$ to $|s'|$ $s'_{i-1} \le s'_i$.</p><p>Does there exist such a sequence $a$ that the resulting string $s'$ is sorted?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains a string $s$ ($2 \le |s| \le 100$). Each character is either '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p></div><div class="output-specification"><p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists a sequence $a$ such that removing the characters at positions $a_1, a_2, \dots, a_k$ and concatenating the parts without changing the order produces a sorted string.</p><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains a string $s$ ($2 \le |s| \le 100$). Each character is either '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p>

## Output

<p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists a sequence $a$ such that removing the characters at positions $a_1, a_2, \dots, a_k$ and concatenating the parts without changing the order produces a sorted string.</p><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>





```input1
5
10101011011
0000
11111
110
1100
```




```output1
YES
YES
YES
YES
NO
```



## Note

<p>In the first testcase you can choose a sequence $a=[1,3,6,9]$. Removing the underlined letters from "<span class="tex-font-style-tt"><span class="tex-font-style-underline">1</span>0<span class="tex-font-style-underline">1</span>01<span class="tex-font-style-underline">0</span>11<span class="tex-font-style-underline">0</span>11</span>" will produce a string "<span class="tex-font-style-tt">0011111</span>", which is sorted.</p><p>In the second and the third testcases the sequences are already sorted.</p><p>In the fourth testcase you can choose a sequence $a=[3]$. $s'=$ "<span class="tex-font-style-tt">11</span>", which is sorted.</p><p>In the fifth testcase there is no way to choose a sequence $a$ such that $s'$ is sorted.</p>
