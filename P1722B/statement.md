## Description

<div><p>Vasya has a grid with $2$ rows and $n$ columns. He colours each cell red, green, or blue.</p><p>Vasya is colourblind and can't distinguish green from blue. Determine if Vasya will consider the two rows of the grid to be coloured the same.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of columns of the grid.</p><p>The following two lines each contain a string consisting of $n$ characters, each of which is either <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">G</span>, or <span class="tex-font-style-tt">B</span>, representing a red, green, or blue cell, respectively&nbsp;— the description of the grid.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Vasya considers the grid's two rows to be identical, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of columns of the grid.</p><p>The following two lines each contain a string consisting of $n$ characters, each of which is either <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">G</span>, or <span class="tex-font-style-tt">B</span>, representing a red, green, or blue cell, respectively&nbsp;— the description of the grid.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Vasya considers the grid's two rows to be identical, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,8,9,10,14,15,16
6
2
RG
RB
4
GRBG
GBGB
5
GGGGG
BBBBB
7
BBBBBBB
RRRRRRR
8
RGBRRGBR
RGGRRBGR
1
G
G
```




```output1
YES
NO
YES
NO
YES
YES
```



## Note

<p>In the first test case, Vasya sees the second cell of each row as the same because the second cell of the first row is green and the second cell of the second row is blue, so he can't distinguish these two cells. The rest of the rows are equal in colour. Therefore, Vasya will say that the two rows are coloured the same, even though they aren't.</p><p>In the second test case, Vasya can see that the two rows are different.</p><p>In the third test case, every cell is green or blue, so Vasya will think they are the same.</p>
