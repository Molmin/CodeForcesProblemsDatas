## Description

<div><p>A string is called <span class="tex-font-style-it">square</span> if it is some string written twice in a row. For example, the strings "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">abcabc</span>", "<span class="tex-font-style-tt">abab</span>" and "<span class="tex-font-style-tt">baabaa</span>" are square. But the strings "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">abaaab</span>" and "<span class="tex-font-style-tt">abcdabc</span>" are not square.</p><p>For a given string $s$ determine if it is square.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 100$)&nbsp;—the number of test cases.</p><p>This is followed by $t$ lines, each containing a description of one test case. The given strings consist only of lowercase Latin letters and have lengths between $1$ and $100$ inclusive.</p></div><div class="output-specification"><p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if the string in the corresponding test case is square, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 100$)&nbsp;—the number of test cases.</p><p>This is followed by $t$ lines, each containing a description of one test case. The given strings consist only of lowercase Latin letters and have lengths between $1$ and $100$ inclusive.</p>

## Output

<p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if the string in the corresponding test case is square, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
10
a
aa
aaa
aaaa
abab
abcabc
abacaba
xxyy
xyyx
xyxy
```




```output1
NO
YES
NO
YES
YES
YES
NO
NO
NO
YES
```


