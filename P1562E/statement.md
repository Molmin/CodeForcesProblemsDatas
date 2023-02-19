## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-size-small"> Morning desert sun horizon<p>Rise above the sands of time...</p></span></div><div class="epigraph-source"><span class="tex-font-size-small">Fates Warning, "Exodus"</span></div></div><p>After crossing the Windswept Wastes, Ori has finally reached the Windtorn Ruins to find the Heart of the Forest! However, the ancient repository containing this priceless Willow light did not want to open!</p><p>Ori was taken aback, but the Voice of the Forest explained to him that the cunning Gorleks had decided to add protection to the repository.</p><p>The Gorleks were very fond of the "string expansion" operation. They were also very fond of increasing subsequences.</p><p>Suppose a string $s_1s_2s_3 \ldots s_n$ is given. Then its "expansion" is defined as the sequence of strings $s_1$, $s_1 s_2$, ..., $s_1 s_2 \ldots s_n$, $s_2$, $s_2 s_3$, ..., $s_2 s_3 \ldots s_n$, $s_3$, $s_3 s_4$, ..., $s_{n-1} s_n$, $s_n$. For example, the "expansion" the string '<span class="tex-font-style-tt">abcd</span>' will be the following sequence of strings: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">ab</span>', '<span class="tex-font-style-tt">abc</span>', '<span class="tex-font-style-tt">abcd</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">bc</span>', '<span class="tex-font-style-tt">bcd</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">cd</span>', '<span class="tex-font-style-tt">d</span>'. </p><p>To open the ancient repository, Ori must find the size of the largest increasing subsequence of the "expansion" of the string $s$. Here, strings are compared lexicographically.</p><p>Help Ori with this task!</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$.</li></ul></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($1 \le n \le 5000$)&nbsp;— length of the string.</p><p>The second line of each test case contains a non-empty string of length $n$, which consists of lowercase latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For every test case print one non-negative integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($1 \le n \le 5000$)&nbsp;— length of the string.</p><p>The second line of each test case contains a non-empty string of length $n$, which consists of lowercase latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For every test case print one non-negative integer&nbsp;— the answer to the problem.</p>





```input1
7
5
acbac
8
acabacba
12
aaaaaaaaaaaa
10
abacabadac
8
dcbaabcd
3
cba
6
sparky
```




```output1
9
17
12
29
14
3
9
```



## Note

<p>In first test case the "expansion" of the string is: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">ac</span>', '<span class="tex-font-style-tt">acb</span>', '<span class="tex-font-style-tt">acba</span>', '<span class="tex-font-style-tt">acbac</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">cb</span>', '<span class="tex-font-style-tt">cba</span>', '<span class="tex-font-style-tt">cbac</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">ba</span>', '<span class="tex-font-style-tt">bac</span>', '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">ac</span>', '<span class="tex-font-style-tt">c</span>'. The answer can be, for example, '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">ac</span>', '<span class="tex-font-style-tt">acb</span>', '<span class="tex-font-style-tt">acba</span>', '<span class="tex-font-style-tt">acbac</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">ba</span>', '<span class="tex-font-style-tt">bac</span>', '<span class="tex-font-style-tt">c</span>'.</p>
