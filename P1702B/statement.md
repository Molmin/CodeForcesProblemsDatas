## Description

<div><p>Polycarp has a poor memory. Each day he can remember no more than $3$ of different letters. </p><p>Polycarp wants to write a non-empty string of $s$ consisting of lowercase Latin letters, taking <span class="tex-font-style-bf">minimum</span> number of days. In how many days will he be able to do it?</p><p>Polycarp initially has an empty string and can only add characters to the end of that string.</p><p>For example, if Polycarp wants to write the string <span class="tex-font-style-tt">lollipops</span>, he will do it in $2$ days: </p><ul> <li> on the first day Polycarp will memorize the letters <span class="tex-font-style-tt">l</span>, <span class="tex-font-style-tt">o</span>, <span class="tex-font-style-tt">i</span> and write <span class="tex-font-style-tt">lolli</span>; </li><li> On the second day Polycarp will remember the letters <span class="tex-font-style-tt">p</span>, <span class="tex-font-style-tt">o</span>, <span class="tex-font-style-tt">s</span>, add <span class="tex-font-style-tt">pops</span> to the resulting line and get the line <span class="tex-font-style-tt">lollipops</span>. </li></ul><p>If Polycarp wants to write the string <span class="tex-font-style-tt">stringology</span>, he will do it in $4$ days: </p><ul> <li> in the first day will be written part <span class="tex-font-style-tt">str</span>; </li><li> on day two will be written part <span class="tex-font-style-tt">ing</span>; </li><li> on the third day, part of <span class="tex-font-style-tt">olog</span> will be written; </li><li> on the fourth day, part of <span class="tex-font-style-tt">y</span> will be written. </li></ul><p>For a given string $s$, print the minimum number of days it will take Polycarp to write it.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of a non-empty string $s$ consisting of lowercase Latin letters (the length of the string $s$ does not exceed $2 \cdot 10^5$)&nbsp;— the string Polycarp wants to construct.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single number&nbsp;— <span class="tex-font-style-bf">minimum</span> number of days it will take Polycarp to write the string $s$ from memory.</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of a non-empty string $s$ consisting of lowercase Latin letters (the length of the string $s$ does not exceed $2 \cdot 10^5$)&nbsp;— the string Polycarp wants to construct.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single number&nbsp;— <span class="tex-font-style-bf">minimum</span> number of days it will take Polycarp to write the string $s$ from memory.</p>





```input1|2,4,6
6
lollipops
stringology
abracadabra
codeforces
test
f
```




```output1
2
4
3
4
1
1
```


