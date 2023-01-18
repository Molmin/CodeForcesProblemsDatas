## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> consisting of characters <span class="tex-span">0</span> and <span class="tex-span">1</span>. <span class="tex-span"><i>m</i></span> operations are performed, on each of them you concatenate two existing strings into a new one. On the <span class="tex-span"><i>i</i></span>-th operation the concatenation <span class="tex-span"><i>s</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub><i>s</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub></span> is saved into a new string <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i> + <i>i</i></sub></span> (the operations are numbered starting from <span class="tex-span">1</span>). After each operation you need to find the maximum positive integer <span class="tex-span"><i>k</i></span> such that all possible strings consisting of <span class="tex-span">0</span> and <span class="tex-span">1</span> of length <span class="tex-span"><i>k</i></span> (there are <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> such strings) are substrings of the new string. If there is no such <span class="tex-span"><i>k</i></span>, print <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of strings. The next <span class="tex-span"><i>n</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>), one per line. The total length of strings is not greater than <span class="tex-span">100</span>.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of operations. <span class="tex-span"><i>m</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> abd <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> + <i>i</i> - 1</span>)&nbsp;— the number of strings that are concatenated to form <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i> + <i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, each should contain one integer&nbsp;— the answer to the question after the corresponding operation.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of strings. The next <span class="tex-span"><i>n</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>), one per line. The total length of strings is not greater than <span class="tex-span">100</span>.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of operations. <span class="tex-span"><i>m</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> abd <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> + <i>i</i> - 1</span>)&nbsp;— the number of strings that are concatenated to form <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i> + <i>i</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, each should contain one integer&nbsp;— the answer to the question after the corresponding operation.</p>





```input1
5
01
10
101
11111
0
3
1 2
6 5
4 4

```




```output1
1
2
0

```



## Note

<p>On the first operation, a new string "<span class="tex-font-style-tt">0110</span>" is created. For <span class="tex-span"><i>k</i> = 1</span> the two possible binary strings of length <span class="tex-span"><i>k</i></span> are "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>", they are substrings of the new string. For <span class="tex-span"><i>k</i> = 2</span> and greater there exist strings of length <span class="tex-span"><i>k</i></span> that do not appear in this string (for <span class="tex-span"><i>k</i> = 2</span> such string is "<span class="tex-font-style-tt">00</span>"). So the answer is <span class="tex-span">1</span>.</p><p>On the second operation the string "<span class="tex-font-style-tt">01100</span>" is created. Now all strings of length <span class="tex-span"><i>k</i> = 2</span> are present.</p><p>On the third operation the string "<span class="tex-font-style-tt">1111111111</span>" is created. There is no zero, so the answer is <span class="tex-span">0</span>.</p>
