## Description

<div><p>We start with a string $s$ consisting only of the digits $1$, $2$, or $3$. The length of $s$ is denoted by $|s|$. For each $i$ from $1$ to $|s|$, the $i$-th character of $s$ is denoted by $s_i$. </p><p>There is one cursor. The cursor's location $\ell$ is denoted by an integer in $\{0, \ldots, |s|\}$, with the following meaning: </p><ul> <li> If $\ell = 0$, then the cursor is located before the first character of $s$. </li><li> If $\ell = |s|$, then the cursor is located right after the last character of $s$. </li><li> If $0 &lt; \ell &lt; |s|$, then the cursor is located between $s_\ell$ and $s_{\ell+1}$. </li></ul><p>We denote by $s_\text{left}$ the string to the left of the cursor and $s_\text{right}$ the string to the right of the cursor. </p><p>We also have a string $c$, which we call our <span class="tex-font-style-underline">clipboard</span>, which starts out as empty. There are three types of actions:</p><ul> <li> <span class="tex-font-style-bf">The Move action</span>. Move the cursor one step to the right. This increments $\ell$ once. </li><li> <span class="tex-font-style-bf">The Cut action</span>. Set $c \leftarrow s_\text{right}$, then set $s \leftarrow s_\text{left}$. </li><li> <span class="tex-font-style-bf">The Paste action</span>. Append the value of $c$ to the end of the string $s$. Note that this doesn't modify $c$. </li></ul><p>The cursor initially starts at $\ell = 0$. Then, we perform the following procedure:</p><ol> <li> Perform the Move action once. </li><li> Perform the Cut action once. </li><li> Perform the Paste action $s_\ell$ times. </li><li> If $\ell = x$, stop. Otherwise, return to step 1. </li></ol><p>You're given the initial string $s$ and the integer $x$. What is the length of $s$ when the procedure stops? Since this value may be very large, only find it modulo $10^9 + 7$. </p><p>It is guaranteed that $\ell \le |s|$ at any time.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 1000$) denoting the number of test cases. The next lines contain descriptions of the test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x \le 10^6$). The second line of each test case consists of the initial string $s$ ($1 \le |s| \le 500$). It is guaranteed, that $s$ consists of the characters "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>".</p><p>It is guaranteed that the sum of $x$ in a single file is at most $10^6$. It is guaranteed that in each test case before the procedure will stop it will be true that $\ell \le |s|$ at any time.</p></div><div class="output-specification"><p>For each test case, output a single line containing a single integer denoting the answer for that test case modulo $10^9 + 7$. </p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 1000$) denoting the number of test cases. The next lines contain descriptions of the test cases.</p><p>The first line of each test case contains a single integer $x$ ($1 \le x \le 10^6$). The second line of each test case consists of the initial string $s$ ($1 \le |s| \le 500$). It is guaranteed, that $s$ consists of the characters "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>".</p><p>It is guaranteed that the sum of $x$ in a single file is at most $10^6$. It is guaranteed that in each test case before the procedure will stop it will be true that $\ell \le |s|$ at any time.</p>

## Output

<p>For each test case, output a single line containing a single integer denoting the answer for that test case modulo $10^9 + 7$. </p>





```input1
4
5
231
7
2323
6
333
24
133321333
```




```output1
25
1438
1101
686531475
```



## Note

<p>Let's illustrate what happens with the first test case. Initially, we have $s = $ <span class="tex-font-style-tt">231</span>. Initially, $\ell = 0$ and $c = \varepsilon$ (the empty string). The following things happen if we follow the procedure above:</p><ul><p> </p><li> <span class="tex-font-style-underline">Step 1</span>, <span class="tex-font-style-it">Move once:</span> we get $\ell = 1$. </li><li> <span class="tex-font-style-underline">Step 2</span>, <span class="tex-font-style-it">Cut once:</span> we get $s = $ <span class="tex-font-style-tt">2</span> and $c = $ <span class="tex-font-style-tt">31</span>. </li><li> <span class="tex-font-style-underline">Step 3</span>, <span class="tex-font-style-it">Paste $s_\ell = $ <span class="tex-font-style-tt">2</span> times:</span> we get $s = $ <span class="tex-font-style-tt">23131</span>. </li><li> <span class="tex-font-style-underline">Step 4</span>: $\ell = 1 \not= x = 5$, so we return to step 1. <p> </p></li><li> <span class="tex-font-style-underline">Step 1</span>, <span class="tex-font-style-it">Move once:</span> we get $\ell = 2$. </li><li> <span class="tex-font-style-underline">Step 2</span>, <span class="tex-font-style-it">Cut once:</span> we get $s = $ <span class="tex-font-style-tt">23</span> and $c = $ <span class="tex-font-style-tt">131</span>. </li><li> <span class="tex-font-style-underline">Step 3</span>, <span class="tex-font-style-it">Paste $s_\ell = $ <span class="tex-font-style-tt">3</span> times:</span> we get $s = $ <span class="tex-font-style-tt">23131131131</span>. </li><li> <span class="tex-font-style-underline">Step 4</span>: $\ell = 2 \not= x = 5$, so we return to step 1. <p> </p></li><li> <span class="tex-font-style-underline">Step 1</span>, <span class="tex-font-style-it">Move once:</span> we get $\ell = 3$. </li><li> <span class="tex-font-style-underline">Step 2</span>, <span class="tex-font-style-it">Cut once:</span> we get $s = $ <span class="tex-font-style-tt">231</span> and $c = $ <span class="tex-font-style-tt">31131131</span>. </li><li> <span class="tex-font-style-underline">Step 3</span>, <span class="tex-font-style-it">Paste $s_\ell = $ <span class="tex-font-style-tt">1</span> time:</span> we get $s = $ <span class="tex-font-style-tt">23131131131</span>. </li><li> <span class="tex-font-style-underline">Step 4</span>: $\ell = 3 \not= x = 5$, so we return to step 1. <p> </p></li><li> <span class="tex-font-style-underline">Step 1</span>, <span class="tex-font-style-it">Move once:</span> we get $\ell = 4$. </li><li> <span class="tex-font-style-underline">Step 2</span>, <span class="tex-font-style-it">Cut once:</span> we get $s = $ <span class="tex-font-style-tt">2313</span> and $c = $ <span class="tex-font-style-tt">1131131</span>. </li><li> <span class="tex-font-style-underline">Step 3</span>, <span class="tex-font-style-it">Paste $s_\ell = $ <span class="tex-font-style-tt">3</span> times:</span> we get $s = $ <span class="tex-font-style-tt">2313113113111311311131131</span>. </li><li> <span class="tex-font-style-underline">Step 4</span>: $\ell = 4 \not= x = 5$, so we return to step 1. <p> </p></li><li> <span class="tex-font-style-underline">Step 1</span>, <span class="tex-font-style-it">Move once:</span> we get $\ell = 5$. </li><li> <span class="tex-font-style-underline">Step 2</span>, <span class="tex-font-style-it">Cut once:</span> we get $s = $ <span class="tex-font-style-tt">23131</span> and $c = $ <span class="tex-font-style-tt">13113111311311131131</span>. </li><li> <span class="tex-font-style-underline">Step 3</span>, <span class="tex-font-style-it">Paste $s_\ell = $ <span class="tex-font-style-tt">1</span> times:</span> we get $s = $ <span class="tex-font-style-tt">2313113113111311311131131</span>. </li><li> <span class="tex-font-style-underline">Step 4</span>: $\ell = 5 = x$, so we stop. </li></ul><p>At the end of the procedure, $s$ has length $25$. </p>
