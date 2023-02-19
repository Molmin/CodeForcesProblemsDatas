## Description

<div><p>You have a string $s$ and a chip, which you can place onto any character of this string. </p><p>After placing the chip, you move it to the right several (maybe zero) times, i.&nbsp;e. you perform the following operation several times: if the current position of the chip is $i$, you move it to the position $i + 1$. Of course, moving the chip to the right is impossible if it is already in the last position.</p><p>After moving the chip to the right, you move it to the left several (maybe zero) times, i.&nbsp;e. you perform the following operation several times: if the current position of the chip is $i$, you move it to the position $i - 1$. Of course, moving the chip to the left is impossible if it is already in the first position.</p><p>When you place a chip or move it, you write down the character where the chip ends up after your action. For example, if $s$ is <span class="tex-font-style-tt">abcdef</span>, you place the chip onto the $3$-rd character, move it to the right $2$ times and then move it to the left $3$ times, you write down the string <span class="tex-font-style-tt">cdedcb</span>.</p><p>You are given two strings $s$ and $t$. Your task is to determine whether it's possible to perform the described operations with $s$ so that you write down the string $t$ as a result.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains the string $s$ ($1 \le |s| \le 500$), the second line contains the string $t$ ($1 \le |t| \le 2 \cdot |s| - 1$). Both strings consist of lowercase English characters.</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if you can obtain the string $t$ by performing the process mentioned in the statement with the string $s$, or "<span class="tex-font-style-tt">NO</span>" if you cannot.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains the string $s$ ($1 \le |s| \le 500$), the second line contains the string $t$ ($1 \le |t| \le 2 \cdot |s| - 1$). Both strings consist of lowercase English characters.</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if you can obtain the string $t$ by performing the process mentioned in the statement with the string $s$, or "<span class="tex-font-style-tt">NO</span>" if you cannot.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p>





```input1
6
abcdef
cdedcb
aaa
aaaaa
aab
baaa
ab
b
abcdef
abcdef
ba
baa
```




```output1
YES
YES
NO
YES
YES
NO
```



## Note

<p>Consider the examples.</p><p>The first test case is described in the statement.</p><p>In the second test case, you can place the chip on the $1$-st position, move it twice to the right, and then move it twice to the left.</p><p>In the fourth test case, you can place the chip on the $2$-nd position, and then don't move it at all.</p><p>In the fifth test case, you can place the chip on the $1$-st position, move it $5$ times to the right, and then finish the process.</p>
