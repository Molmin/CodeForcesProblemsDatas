## Description

<div><div class="epigraph"><div class="epigraph-text">Is it really?! The robot only existing in my imagination?! The Colossal Walking Robot?!!</div><div class="epigraph-source">— Kochiya Sanae</div></div> Sanae made a giant robot — Hisoutensoku, but something is wrong with it. To make matters worse, Sanae can not figure out how to stop it, and she is forced to fix it on-the-fly.<p>The state of a robot can be represented by an array of integers of length $n$. Initially, the robot is at state $a$. She wishes to turn it into state $b$. </p><p>As a great programmer, Sanae knows the art of copy-and-paste. In one operation, she can choose some segment from given segments, copy the segment from $b$ and paste it into <span class="tex-font-style-bf">the same place</span> of the robot, replacing the original state there. However, she has to ensure that the sum of $a$ <span class="tex-font-style-bf">does not change</span> after each copy operation in case the robot go haywire. Formally, Sanae can choose segment $[l,r]$ and assign $a_i = b_i$ ($l\le i\le r$) if $\sum\limits_{i=1}^n a_i$ does not change after the operation.</p><p>Determine whether it is possible for Sanae to successfully turn the robot from the initial state $a$ to the desired state $b$ with any (possibly, zero) operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$) — the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \leq n\leq 2\cdot 10^5$, $1 \leq m\leq 2\cdot 10^5$) — the length of $a$, $b$ and the number of segments.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^9$) — the initial state $a$.</p><p>The third line contains $n$ intergers $b_1,b_2,\ldots,b_n$ ($1 \leq b_i \leq 10^9$) — the desired state $b$.</p><p>Then $m$ lines follow, the $i$-th line contains two intergers $l_i,r_i$ ($1 \leq l_i &lt; r_i \leq n$) — the segments that can be copy-pasted by Sanae.</p><p>It is guaranteed that both the sum of $n$ and the sum of $m$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if $a$ can be turned into $b$, or "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$) — the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \leq n\leq 2\cdot 10^5$, $1 \leq m\leq 2\cdot 10^5$) — the length of $a$, $b$ and the number of segments.</p><p>The second line contains $n$ intergers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^9$) — the initial state $a$.</p><p>The third line contains $n$ intergers $b_1,b_2,\ldots,b_n$ ($1 \leq b_i \leq 10^9$) — the desired state $b$.</p><p>Then $m$ lines follow, the $i$-th line contains two intergers $l_i,r_i$ ($1 \leq l_i &lt; r_i \leq n$) — the segments that can be copy-pasted by Sanae.</p><p>It is guaranteed that both the sum of $n$ and the sum of $m$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if $a$ can be turned into $b$, or "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|
2
5 2
1 5 4 2 3
3 2 5 4 1
1 3
2 5
5 2
1 5 4 2 3
3 2 4 5 1
1 2
2 4
```




```output1
YES
NO
```



## Note

<p>Test case 1:</p><p>One possible way of turning $a$ to $b$:</p><p>First, select $[1,3]$. After the operation, $a=[3,2,5,2,3]$.</p><p>Then, select $[2,5]$. After the operation, $a=[3,2,5,4,1]=b$.</p><p>Test case 2:</p><p>It can be shown that it is impossible to turn $a$ into $b$. </p>
