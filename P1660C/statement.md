## Description

<div><p>A string $a=a_1a_2\dots a_n$ is called <span class="tex-font-style-it">even</span> if it consists of a concatenation (joining) of strings of length $2$ consisting of the same characters. In other words, a string $a$ is even if two conditions are satisfied <span class="tex-font-style-bf">at the same time</span>:</p><ul> <li> its length $n$ is even; </li><li> for all odd $i$ ($1 \le i \le n - 1$), $a_i = a_{i+1}$ is satisfied. </li></ul><p>For example, the following strings are even: "<span class="tex-font-style-tt"></span>" (empty string), "<span class="tex-font-style-tt">tt</span>", "<span class="tex-font-style-tt">aabb</span>", "<span class="tex-font-style-tt">oooo</span>", and "<span class="tex-font-style-tt">ttrrrroouuuuuuuukk</span>". The following strings are not even: "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">abab</span>" and "<span class="tex-font-style-tt">abba</span>".</p><p>Given a string $s$ consisting of lowercase Latin letters. Find the minimum number of characters to remove from the string $s$ to make it even. The deleted characters do not have to be consecutive.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>Each test case consists of one string $s$ ($1 \le |s| \le 2 \cdot 10^5$), where $|s|$&nbsp;— the length of the string $s$. The string consists of lowercase Latin letters.</p><p>It is guaranteed that the sum of $|s|$ on all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single number&nbsp;— the minimum number of characters that must be removed to make $s$ even.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>Each test case consists of one string $s$ ($1 \le |s| \le 2 \cdot 10^5$), where $|s|$&nbsp;— the length of the string $s$. The string consists of lowercase Latin letters.</p><p>It is guaranteed that the sum of $|s|$ on all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single number&nbsp;— the minimum number of characters that must be removed to make $s$ even.</p>





```input1
6
aabbdabdccc
zyx
aaababbb
aabbcc
oaoaaaoo
bmefbmuyw
```




```output1
3
3
2
0
2
7
```



## Note

<p>In the first test case you can remove the characters with indices $6$, $7$, and $9$ to get an even string "<span class="tex-font-style-tt">aabbddcc</span>".</p><p>In the second test case, each character occurs exactly once, so in order to get an even string, you must remove all characters from the string.</p><p>In the third test case, you can get an even string "<span class="tex-font-style-tt">aaaabb</span>" by removing, for example, $4$-th and $6$-th characters, or a string "<span class="tex-font-style-tt">aabbbb</span>" by removing the $5$-th character and any of the first three.</p>
