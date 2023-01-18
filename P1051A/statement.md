## Description

<div><p>Vasya came up with a password to register for <span class="tex-font-style-it">EatForces</span> — a string $s$. The password in <span class="tex-font-style-it">EatForces</span> should be a string, consisting of lowercase and uppercase Latin letters and digits.</p><p>But since <span class="tex-font-style-it">EatForces</span> takes care of the security of its users, user passwords must contain at least one digit, at least one uppercase Latin letter and at least one lowercase Latin letter. For example, the passwords "<span class="tex-font-style-tt">abaCABA12</span>", "<span class="tex-font-style-tt">Z7q</span>" and "<span class="tex-font-style-tt">3R24m</span>" are valid, and the passwords "<span class="tex-font-style-tt">qwerty</span>", "<span class="tex-font-style-tt">qwerty12345</span>" and "<span class="tex-font-style-tt">Password</span>" are not. </p><p>A substring of string $s$ is a string $x = s_l s_{l + 1} \dots s_{l + len - 1} (1 \le l \le |s|, 0 \le len \le |s| - l + 1)$. $len$ is the length of the substring. Note that the empty string is also considered a substring of $s$, it has the length $0$.</p><p>Vasya's password, however, may come too weak for the security settings of <span class="tex-font-style-it">EatForces</span>. He likes his password, so he wants to replace some its substring with another string of the same length in order to satisfy the above conditions. This operation should be performed <span class="tex-font-style-bf">exactly</span> once, and <span class="tex-font-style-bf">the chosen string should have the minimal possible length</span>.</p><p><span class="tex-font-style-bf">Note that the length of $s$ should not change after the replacement of the substring, and the string itself should contain only lowercase and uppercase Latin letters and digits.</span></p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of testcases.</p><p>Each of the next $T$ lines contains the initial password $s~(3 \le |s| \le 100)$, consisting of lowercase and uppercase Latin letters and digits.</p><p><span class="tex-font-style-bf">Only $T = 1$ is allowed for hacks</span>.</p></div><div class="output-specification"><p>For each testcase print a renewed password, which corresponds to given conditions. </p><p>The length of the replaced substring is calculated as following: write down all the changed positions. If there are none, then the length is $0$. Otherwise the length is the difference between the first and the last changed position plus one. For example, the length of the changed substring between the passwords "<span class="tex-font-style-tt">abcdef</span>" $\rightarrow$ "<span class="tex-font-style-tt">a7cdEf</span>" is $4$, because the changed positions are $2$ and $5$, thus $(5 - 2) + 1 = 4$.</p><p><span class="tex-font-style-bf">It is guaranteed that such a password always exists.</span></p><p>If there are several suitable passwords — output any of them.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of testcases.</p><p>Each of the next $T$ lines contains the initial password $s~(3 \le |s| \le 100)$, consisting of lowercase and uppercase Latin letters and digits.</p><p><span class="tex-font-style-bf">Only $T = 1$ is allowed for hacks</span>.</p>

## Output

<p>For each testcase print a renewed password, which corresponds to given conditions. </p><p>The length of the replaced substring is calculated as following: write down all the changed positions. If there are none, then the length is $0$. Otherwise the length is the difference between the first and the last changed position plus one. For example, the length of the changed substring between the passwords "<span class="tex-font-style-tt">abcdef</span>" $\rightarrow$ "<span class="tex-font-style-tt">a7cdEf</span>" is $4$, because the changed positions are $2$ and $5$, thus $(5 - 2) + 1 = 4$.</p><p><span class="tex-font-style-bf">It is guaranteed that such a password always exists.</span></p><p>If there are several suitable passwords — output any of them.</p>





```input1
2
abcDCE
htQw27

```




```output1
abcD4E
htQw27

```



## Note

<p>In the first example Vasya's password lacks a digit, he replaces substring "<span class="tex-font-style-tt">C</span>" with "<span class="tex-font-style-tt">4</span>" and gets password "abcD4E". That means, he changed the substring of length 1.</p><p>In the second example Vasya's password is ok from the beginning, and nothing has to be changed. That is the same as replacing the empty substring with another empty substring (length 0).</p>
