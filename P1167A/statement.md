## Description

<div><p>A telephone number is a sequence of exactly <span class="tex-font-style-tt">11</span> digits, where the first digit is <span class="tex-font-style-tt">8</span>. For example, the sequence <span class="tex-font-style-tt">80011223388</span> is a telephone number, but the sequences <span class="tex-font-style-tt">70011223388</span> and <span class="tex-font-style-tt">80000011223388</span> are not.</p><p>You are given a string $s$ of length $n$, consisting of digits.</p><p>In one operation you can delete any character from string $s$. For example, it is possible to obtain strings <span class="tex-font-style-tt">112</span>, <span class="tex-font-style-tt">111</span> or <span class="tex-font-style-tt">121</span> from string <span class="tex-font-style-tt">1121</span>.</p><p>You need to determine whether there is such a sequence of operations (possibly empty), after which the string $s$ becomes a telephone number.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$) — the length of string $s$.</p><p>The second line of each test case contains the string $s$ ($|s| = n$) consisting of digits.</p></div><div class="output-specification"><p>For each test print one line.</p><p>If there is a sequence of operations, after which $s$ becomes a telephone number, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$) — the length of string $s$.</p><p>The second line of each test case contains the string $s$ ($|s| = n$) consisting of digits.</p>

## Output

<p>For each test print one line.</p><p>If there is a sequence of operations, after which $s$ becomes a telephone number, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
2
13
7818005553535
11
31415926535
```




```output1
YES
NO
```



## Note

<p>In the first test case you need to delete the first and the third digits. Then the string <span class="tex-font-style-tt">7818005553535</span> becomes <span class="tex-font-style-tt">88005553535</span>.</p>
