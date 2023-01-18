## Description

<div><p>Vasya's birthday is approaching and Lena decided to sew a patterned handkerchief to him as a present. Lena chose digits from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> as the pattern. The digits will form a rhombus. The largest digit <span class="tex-span"><i>n</i></span> should be located in the centre. The digits should decrease as they approach the edges. For example, for <span class="tex-span"><i>n</i> = 5</span> the handkerchief pattern should look like that: </p><pre class="verbatim"><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;3&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;3&nbsp;4&nbsp;3&nbsp;2&nbsp;1&nbsp;0<br>0&nbsp;1&nbsp;2&nbsp;3&nbsp;4&nbsp;5&nbsp;4&nbsp;3&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;3&nbsp;4&nbsp;3&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;3&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;2&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0&nbsp;1&nbsp;0<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0<br></pre><p>Your task is to determine the way the handkerchief will look like by the given <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 9</span>).</p></div><div class="output-specification"><p>Print a picture for the given <span class="tex-span"><i>n</i></span>. You should strictly observe the number of spaces before the first digit on each line. Every two adjacent digits in the same line should be separated by exactly one space. There should be no spaces after the last digit at the end of each line.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 9</span>).</p>

## Output

<p>Print a picture for the given <span class="tex-span"><i>n</i></span>. You should strictly observe the number of spaces before the first digit on each line. Every two adjacent digits in the same line should be separated by exactly one space. There should be no spaces after the last digit at the end of each line.</p>





```input1
2

```




```input2
3

```




```output1
0
  0 1 0
0 1 2 1 0
  0 1 0
    0

```




```output2
0
    0 1 0
  0 1 2 1 0
0 1 2 3 2 1 0
  0 1 2 1 0
    0 1 0
      0

```


