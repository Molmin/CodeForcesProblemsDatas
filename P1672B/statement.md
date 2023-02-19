## Description

<div><p>Let's call a string <span class="tex-font-style-bf">good</span> if its length is at least $2$ and all of its characters are $\texttt{A}$ except for the last character which is $\texttt{B}$. The good strings are $\texttt{AB},\texttt{AAB},\texttt{AAAB},\ldots$. Note that $\texttt{B}$ is <span class="tex-font-style-bf">not</span> a good string.</p><p>You are given an initially empty string $s_1$.</p><p>You can perform the following operation any number of times: </p><ul> <li> Choose any position of $s_1$ and insert some good string in that position. </li></ul><p>Given a string $s_2$, can we turn $s_1$ into $s_2$ after some number of operations?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single string $s_2$ ($1 \leq |s_2| \leq 2 \cdot 10^5$).</p><p>It is guaranteed that $s_2$ consists of only the characters $\texttt{A}$ and $\texttt{B}$.</p><p>It is guaranteed that the sum of $|s_2|$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if we can turn $s_1$ into $s_2$ after some number of operations, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single string $s_2$ ($1 \leq |s_2| \leq 2 \cdot 10^5$).</p><p>It is guaranteed that $s_2$ consists of only the characters $\texttt{A}$ and $\texttt{B}$.</p><p>It is guaranteed that the sum of $|s_2|$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if we can turn $s_1$ into $s_2$ after some number of operations, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,4
4
AABAB
ABB
AAAAAAAAB
A
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first test case, we transform $s_1$ as such: $\varnothing \to \color{red}{\texttt{AAB}} \to \texttt{A}\color{red}{\texttt{AB}}\texttt{AB}$.</p><p>In the third test case, we transform $s_1$ as such: $\varnothing \to \color{red}{\texttt{AAAAAAAAB}}$.</p><p>In the second and fourth test case, it can be shown that it is impossible to turn $s_1$ into $s_2$.</p>
