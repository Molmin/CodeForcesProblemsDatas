## Description

<div><p>You are given strings $S$ and $T$, consisting of lowercase English letters. It is guaranteed that $T$ is a permutation of the string <span class="tex-font-style-tt">abc</span>. </p><p>Find string $S'$, the <span class="tex-font-style-bf">lexicographically smallest</span> permutation of $S$ such that $T$ is <span class="tex-font-style-bf">not</span> a subsequence of $S'$.</p><p>String $a$ is a <span class="tex-font-style-it">permutation</span> of string $b$ if the number of occurrences of each distinct character is the same in both strings.</p><p>A string $a$ is a <span class="tex-font-style-it">subsequence</span> of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p><p>A string $a$ is <span class="tex-font-style-it">lexicographically smaller</span> than a string $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$.</li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a string $S$ ($1 \le |S| \le 100$), consisting of lowercase English letters.</p><p>The second line of each test case contains a string $T$ that is a permutation of the string <span class="tex-font-style-tt">abc</span>. (Hence, $|T| = 3$).</p><p>Note that there is no limit on the sum of $|S|$ across all test cases.</p></div><div class="output-specification"><p>For each test case, output a single string $S'$, the lexicographically smallest permutation of $S$ such that $T$ is not a subsequence of $S'$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a string $S$ ($1 \le |S| \le 100$), consisting of lowercase English letters.</p><p>The second line of each test case contains a string $T$ that is a permutation of the string <span class="tex-font-style-tt">abc</span>. (Hence, $|T| = 3$).</p><p>Note that there is no limit on the sum of $|S|$ across all test cases.</p>

## Output

<p>For each test case, output a single string $S'$, the lexicographically smallest permutation of $S$ such that $T$ is not a subsequence of $S'$.</p>





```input1
7
abacaba
abc
cccba
acb
dbsic
bac
abracadabra
abc
dddddddddddd
cba
bbc
abc
ac
abc
```




```output1
aaaacbb
abccc
bcdis
aaaaacbbdrr
dddddddddddd
bbc
ac
```



## Note

<p>In the first test case, both <span class="tex-font-style-tt">aaaabbc</span> and <span class="tex-font-style-tt">aaaabcb</span> are lexicographically smaller than <span class="tex-font-style-tt">aaaacbb</span>, but they contain <span class="tex-font-style-tt">abc</span> as a subsequence.</p><p>In the second test case, <span class="tex-font-style-tt">abccc</span> is the smallest permutation of <span class="tex-font-style-tt">cccba</span> and does not contain <span class="tex-font-style-tt">acb</span> as a subsequence.</p><p>In the third test case, <span class="tex-font-style-tt">bcdis</span> is the smallest permutation of <span class="tex-font-style-tt">dbsic</span> and does not contain <span class="tex-font-style-tt">bac</span> as a subsequence.</p>
