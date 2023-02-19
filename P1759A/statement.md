## Description

<div><p>You talked to Polycarp and asked him a question. You know that when he wants to answer "yes", he repeats <span class="tex-font-style-tt">Yes</span> many times in a row.</p><p>Because of the noise, you only heard part of the answer&nbsp;— some substring of it. That is, if he answered <span class="tex-font-style-tt">YesYes</span>, then you could hear <span class="tex-font-style-tt">esY</span>, <span class="tex-font-style-tt">YesYes</span>, <span class="tex-font-style-tt">sYes</span>, <span class="tex-font-style-tt">e</span>, but you couldn't <span class="tex-font-style-tt">Yess</span>, <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">se</span>.</p><p>Determine if it is true that the given string $s$ is a substring of <span class="tex-font-style-tt">YesYesYes...</span> (<span class="tex-font-style-tt">Yes</span> repeated many times in a row).</p></div><div class="input-specification"><p>The first line of input data contains the singular $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the test.</p><p>Each test case is described by a single string of Latin letters $s$ ($1 \le |s| \le 50$)&nbsp;— the part of Polycarp's answer that you heard, where $|s|$ — is the length of the string $s$.</p></div><div class="output-specification"><p>Output $t$ lines, each of which is the answer to the corresponding test case. As an answer, output "<span class="tex-font-style-tt">YES</span>" if the specified string $s$ is a substring of the string <span class="tex-font-style-tt">YesYesYes...Yes</span> (the number of words <span class="tex-font-style-tt">Yes</span> is arbitrary), and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of input data contains the singular $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the test.</p><p>Each test case is described by a single string of Latin letters $s$ ($1 \le |s| \le 50$)&nbsp;— the part of Polycarp's answer that you heard, where $|s|$ — is the length of the string $s$.</p>

## Output

<p>Output $t$ lines, each of which is the answer to the corresponding test case. As an answer, output "<span class="tex-font-style-tt">YES</span>" if the specified string $s$ is a substring of the string <span class="tex-font-style-tt">YesYesYes...Yes</span> (the number of words <span class="tex-font-style-tt">Yes</span> is arbitrary), and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,4,6,8,10,12
12
YES
esYes
codeforces
es
se
YesY
esYesYesYesYesYesYe
seY
Yess
sY
o
Yes
```




```output1
NO
YES
NO
YES
NO
YES
YES
NO
NO
YES
NO
YES
```


