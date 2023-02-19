## Description

<div><p>Timur likes his name. As a spelling of his name, he allows any permutation of the letters of the name. For example, the following strings are valid spellings of his name: <span class="tex-font-style-tt">Timur</span>, <span class="tex-font-style-tt">miurT</span>, <span class="tex-font-style-tt">Trumi</span>, <span class="tex-font-style-tt">mriTu</span>. Note that the correct spelling must have uppercased <span class="tex-font-style-tt">T</span> and lowercased other letters.</p><p>Today he wrote string $s$ of length $n$ consisting only of uppercase or lowercase Latin letters. He asks you to check if $s$ is the correct spelling of his name.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ $(1 \leq n \leq 10)$&nbsp;— the length of string $s$.</p><p>The second line of each test case contains a string $s$ consisting of only uppercase or lowercase Latin characters.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $s$ satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ $(1 \leq n \leq 10)$&nbsp;— the length of string $s$.</p><p>The second line of each test case contains a string $s$ consisting of only uppercase or lowercase Latin characters.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $s$ satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
5
Timur
5
miurT
5
Trumi
5
mriTu
5
timur
4
Timr
6
Timuur
10
codeforces
10
TimurTimur
5
TIMUR
```




```output1
YES
YES
YES
YES
NO
NO
NO
NO
NO
NO
```


