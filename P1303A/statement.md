## Description

<div><p>You are given a string $s$. Each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p><p>You want all <span class="tex-font-style-tt">1</span>'s in the string to form a contiguous subsegment. For example, if the string is <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">00111</span> or <span class="tex-font-style-tt">01111100</span>, then all <span class="tex-font-style-tt">1</span>'s form a contiguous subsegment, and if the string is <span class="tex-font-style-tt">0101</span>, <span class="tex-font-style-tt">100001</span> or <span class="tex-font-style-tt">11111111111101</span>, then this condition is not met.</p><p>You may erase some (possibly none) <span class="tex-font-style-tt">0</span>'s from the string. What is the minimum number of <span class="tex-font-style-tt">0</span>'s that you have to erase?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then $t$ lines follow, each representing a test case. Each line contains one string $s$ ($1 \le |s| \le 100$); each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print $t$ integers, where the $i$-th integer is the answer to the $i$-th testcase (the minimum number of <span class="tex-font-style-tt">0</span>'s that you have to erase from $s$).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then $t$ lines follow, each representing a test case. Each line contains one string $s$ ($1 \le |s| \le 100$); each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print $t$ integers, where the $i$-th integer is the answer to the $i$-th testcase (the minimum number of <span class="tex-font-style-tt">0</span>'s that you have to erase from $s$).</p>





```input1
3
010011
0
1111000
```




```output1
2
0
0
```



## Note

<p>In the first test case you have to delete the third and forth symbols from string <span class="tex-font-style-tt">010011</span> (it turns into <span class="tex-font-style-tt">0111</span>).</p>
