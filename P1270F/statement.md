## Description

<div><p>Let's call a binary string $s$ <span class="tex-font-style-bf">awesome</span>, if it has at least $1$ symbol <span class="tex-font-style-tt">1</span> and length of the string is divisible by the number of <span class="tex-font-style-tt">1</span> in it. In particular, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">1010</span>, <span class="tex-font-style-tt">111</span> are <span class="tex-font-style-bf">awesome</span>, but <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">110</span>, <span class="tex-font-style-tt">01010</span> aren't.</p><p>You are given a binary string $s$. Count the number of its <span class="tex-font-style-bf">awesome</span> substrings.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>The first line contains the string $s$ ($1 \leq |s|\le 200\,000$) consisting only of zeros and ones.</p></div><div class="output-specification"><p>Output a single number&nbsp;— the number of <span class="tex-font-style-bf">awesome</span> substrings of $s$.</p></div>

## Input

<p>The first line contains the string $s$ ($1 \leq |s|\le 200\,000$) consisting only of zeros and ones.</p>

## Output

<p>Output a single number&nbsp;— the number of <span class="tex-font-style-bf">awesome</span> substrings of $s$.</p>





```input1
111
```




```input2
01010
```




```input3
0000
```




```input4
1111100000
```




```output1
6
```




```output2
10
```




```output3
0
```




```output4
25
```



## Note

<p>In the first sample, all substrings of $s$ are <span class="tex-font-style-bf">awesome</span>.</p><p>In the second sample, we have the following <span class="tex-font-style-bf">awesome</span> substrings of $s$: <span class="tex-font-style-tt">1</span> ($2$ times), <span class="tex-font-style-tt">01</span> ($2$ times), <span class="tex-font-style-tt">10</span> ($2$ times), <span class="tex-font-style-tt">010</span> ($2$ times), <span class="tex-font-style-tt">1010</span>, <span class="tex-font-style-tt">0101</span></p><p>In the third sample, no substring is <span class="tex-font-style-bf">awesome</span>.</p>
