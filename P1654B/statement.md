## Description

<div><p>You are given a string $s$ consisting of lowercase letters of the English alphabet. You must perform the following algorithm on $s$:</p><ul> <li> Let $x$ be the length of the longest prefix of $s$ which occurs somewhere else in $s$ as a contiguous substring (the other occurrence may also intersect the prefix). If $x = 0$, break. Otherwise, remove the first $x$ characters of $s$, and repeat. </li></ul><p>A prefix is a string consisting of several first letters of a given string, without any reorders. An empty prefix is also a valid prefix. For example, the string "<span class="tex-font-style-tt">abcd</span>" has 5 prefixes: empty string, "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">abc</span>" and "<span class="tex-font-style-tt">abcd</span>".</p><p>For instance, if we perform the algorithm on $s =$ "<span class="tex-font-style-tt">abcabdc</span>", </p><ul> <li> Initially, "<span class="tex-font-style-tt">ab</span>" is the longest prefix that also appears somewhere else as a substring in $s$, so $s =$ "<span class="tex-font-style-tt">cabdc</span>" after $1$ operation. </li><li> Then, "<span class="tex-font-style-tt">c</span>" is the longest prefix that also appears somewhere else as a substring in $s$, so $s =$ "<span class="tex-font-style-tt">abdc</span>" after $2$ operations. </li><li> Now $x=0$ (because there are no non-empty prefixes of "<span class="tex-font-style-tt">abdc</span>" that also appear somewhere else as a substring in $s$), so the algorithm terminates. </li></ul><p>Find the final state of the string after performing the algorithm.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>This is followed by $t$ lines, each containing a description of one test case. Each line contains a string $s$. The given strings consist only of lowercase letters of the English alphabet and have lengths between $1$ and $2 \cdot 10^5$ inclusive.</p><p>It is guaranteed that the sum of the lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing the string $s$ after executing the algorithm. It can be shown that such string is non-empty.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>This is followed by $t$ lines, each containing a description of one test case. Each line contains a string $s$. The given strings consist only of lowercase letters of the English alphabet and have lengths between $1$ and $2 \cdot 10^5$ inclusive.</p><p>It is guaranteed that the sum of the lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line containing the string $s$ after executing the algorithm. It can be shown that such string is non-empty.</p>





```input1
6
abcabdc
a
bbbbbbbbbb
codeforces
cffcfccffccfcffcfccfcffccffcfccf
zyzyzwxxyyxxyyzzyzzxxwzxwywxwzxxyzzw
```




```output1
abdc
a
b
deforces
cf
xyzzw
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case, no operations can be performed on $s$.</p><p>In the third test case, </p><ul> <li> Initially, $s =$ "<span class="tex-font-style-tt">bbbbbbbbbb</span>". </li><li> After $1$ operation, $s =$ "<span class="tex-font-style-tt">b</span>". </li></ul><p>In the fourth test case, </p><ul> <li> Initially, $s =$ "<span class="tex-font-style-tt">codeforces</span>". </li><li> After $1$ operation, $s =$ "<span class="tex-font-style-tt">odeforces</span>". </li><li> After $2$ operations, $s =$ "<span class="tex-font-style-tt">deforces</span>". </li></ul>
