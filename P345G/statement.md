## Description

<div><p>You are given a group of <span class="tex-span"><i>n</i></span> strings: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>You should find a subgroup <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub></span> <span class="tex-span">(1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>)</span> of the group. The following two conditions must hold:</p><ul> <li> there exists a string <span class="tex-span"><i>t</i></span> such, that each string from found subgroup is its suffix; </li><li> the number of strings in the found subgroup is as large as possible. </li></ul><p>Your task is to print the number of strings in the found subgroup.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of strings in the group. Each of the next <span class="tex-span"><i>n</i></span> lines contains a string. The <span class="tex-span"><i>i</i></span>-th line contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each string consists only from lowercase Latin letters. The sum of all strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Output a single integer — the number of strings in the found subgroup.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of strings in the group. Each of the next <span class="tex-span"><i>n</i></span> lines contains a string. The <span class="tex-span"><i>i</i></span>-th line contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each string consists only from lowercase Latin letters. The sum of all strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Output a single integer — the number of strings in the found subgroup.</p>





```input1
6
bb
bb
b
aaa
aa
z

```




```output1
3

```



## Note

<p>Look at the test sample. The required subgroup is <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub></span>.</p>
