## Description

<div><p>There is a string $s$ of length $3$, consisting of uppercase and lowercase English letters. Check if it is equal to "<span class="tex-font-style-tt">YES</span>" (without quotes), where each letter can be in any case. For example, "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>" are all allowable.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of testcases.</p><p>The description of each test consists of one line containing one string $s$ consisting of three characters. Each character of $s$ is either an uppercase or lowercase English letter.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $s$ satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of testcases.</p><p>The description of each test consists of one line containing one string $s$ consisting of three characters. Each character of $s$ is either an uppercase or lowercase English letter.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $s$ satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,4,6,8,10
10
YES
yES
yes
Yes
YeS
Noo
orZ
yEz
Yas
XES
```




```output1
YES
YES
YES
YES
YES
NO
NO
NO
NO
NO
```



## Note

<p>The first five test cases contain the strings "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">YeS</span>". All of these are equal to "<span class="tex-font-style-tt">YES</span>", where each character is either uppercase or lowercase.</p>
