## Description

<div><p>You are given an integer $n$. Check if $n$ has an <span class="tex-font-style-bf">odd</span> divisor, greater than one (does there exist such a number $x$ ($x &gt; 1$) that $n$ is divisible by $x$ and $x$ is odd).</p><p>For example, if $n=6$, then there is $x=3$. If $n=4$, then such a number does not exist.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains one integer $n$ ($2 \le n \le 10^{14}$).</p><p>Please note, that the input for some test cases won't fit into $32$-bit integer type, so you should use at least $64$-bit integer type in your programming language.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if $n$ has an <span class="tex-font-style-bf">odd</span> divisor, greater than one; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains one integer $n$ ($2 \le n \le 10^{14}$).</p><p>Please note, that the input for some test cases won't fit into $32$-bit integer type, so you should use at least $64$-bit integer type in your programming language.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if $n$ has an <span class="tex-font-style-bf">odd</span> divisor, greater than one; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p>





```input1
6
2
3
4
5
998244353
1099511627776
```




```output1
NO
YES
NO
YES
YES
NO
```


