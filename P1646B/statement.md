## Description

<div><p>$ \def\myred#1{\color{red}{\underline{\bf{#1}}}} \def\myblue#1{\color{blue}{\overline{\bf{#1}}}} $ $\def\RED{\myred{Red}} \def\BLUE{\myblue{Blue}}$</p><p>You are given a sequence of $n$ non-negative integers $a_1, a_2, \ldots, a_n$. Initially, all the elements of the sequence are unpainted. You can paint each number $\RED$ or $\BLUE$ (but not both), or <span class="tex-font-style-bf">leave it unpainted</span>. </p><p>For a color $c$, $\text{Count}(c)$ is the number of elements in the sequence painted with that color and $\text{Sum}(c)$ is the sum of the elements in the sequence painted with that color.</p><p>For example, if the given sequence is $[2, 8, 6, 3, 1]$ and it is painted this way: $[\myblue{2}, 8, \myred{6}, \myblue{3}, 1]$ (where $6$ is painted red, $2$ and $3$ are painted blue, $1$ and $8$ are unpainted) then $\text{Sum}(\RED)=6$, $\text{Sum}(\BLUE)=2+3=5$, $\text{Count}(\RED)=1$, and $\text{Count}(\BLUE)=2$.</p><p>Determine if it is possible to paint the sequence so that $\text{Sum}(\RED) &gt; \text{Sum}(\BLUE)$ and $\text{Count}(\RED) &lt; \text{Count}(\BLUE)$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3\le n\le 2\cdot 10^5$)&nbsp;— the length of the given sequence. </p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\le a_i\le 10^9$)&nbsp;— the given sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to paint the given sequence satisfying the above requirements, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3\le n\le 2\cdot 10^5$)&nbsp;— the length of the given sequence. </p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\le a_i\le 10^9$)&nbsp;— the given sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to paint the given sequence satisfying the above requirements, and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
4
3
1 2 3
5
2 8 6 3 1
4
3 5 4 2
5
1000000000 1000000000 1000000000 1000000000 1000000000
```




```output1
NO
YES
NO
NO
```



## Note

<p>In the first test case, there is no possible way to paint the sequence. For example, if you paint the sequence this way: $[\myblue{1},\myblue{2},\myred{3}]$ (where $3$ is painted red, $1$ and $2$ are painted blue) then $\text{Count}(\RED)=1 &lt; \text{Count}(\BLUE)=2$, but $\text{Sum}(\RED)=3 \ngtr \text{Sum}(\BLUE)=3$. So, this is not a possible way to paint the sequence.</p><p>In the second test case, a possible way to paint the sequence is described in the statement. We can see that $\text{Sum}(\RED)=6 &gt; \text{Sum}(\BLUE)=5$ and $\text{Count}(\RED)=1 &lt; \text{Count}(\BLUE)=2$.</p><p>In the third test case, there is no possible way to paint the sequence. For example, if you paint the sequence this way: $[\myred{3},\myred{5},\myblue{4}, \myblue{2}]$ (where $3$ and $5$ are painted red, $4$ and $2$ are painted blue) then $\text{Sum}(\RED) = 8 &gt; \text{Sum}(\BLUE) = 6$ but $\text{Count}(\RED) = 2 \nless \text{Count}(\BLUE) = 2$. So, this is not a possible way to paint the sequence.</p><p>In the fourth test case, it can be proven that there is no possible way to paint the sequence satisfying sum and count constraints.</p>
