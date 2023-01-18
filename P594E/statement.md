## Description

<div><p>You are given a non-empty line <span class="tex-span"><i>s</i></span> and an integer <span class="tex-span"><i>k</i></span>. The following operation is performed with this line exactly once:</p><ul> <li> A line is split into <span class="tex-font-style-bf">at most</span> <span class="tex-span"><i>k</i></span> non-empty substrings, i.e. string <span class="tex-span"><i>s</i></span> is represented as a concatenation of a set of strings <span class="tex-span"><i>s</i> = <i>t</i><sub class="lower-index">1</sub> + <i>t</i><sub class="lower-index">2</sub> + ... + <i>t</i><sub class="lower-index"><i>m</i></sub></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>k</i></span>. </li><li> Some of strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are replaced by strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>r</i></sup></span>, that is, their record from right to left. </li><li> The lines are concatenated back in the same order, we get string <span class="tex-span"><i>s</i>' = <i>t</i>'<sub class="lower-index">1</sub><i>t</i>'<sub class="lower-index">2</sub>... <i>t</i>'<sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>t</i>'<sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>r</i></sup></span>. </li></ul><p>Your task is to determine the lexicographically smallest string that could be the result of applying the given operation to the string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5 000 000</span>), consisting of lowercase English letters. The second line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>)&nbsp;— the maximum number of parts in the partition.</p></div><div class="output-specification"><p>In the single line print the lexicographically minimum string <span class="tex-span"><i>s</i>'</span> which can be obtained as a result of performing the described operation. </p></div>

## Input

<p>The first line of the input contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5 000 000</span>), consisting of lowercase English letters. The second line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>)&nbsp;— the maximum number of parts in the partition.</p>

## Output

<p>In the single line print the lexicographically minimum string <span class="tex-span"><i>s</i>'</span> which can be obtained as a result of performing the described operation. </p>





```input1
aba
2

```




```input2
aaaabacaba
2

```




```input3
bababa
1

```




```input4
abacabadabacaba
4

```




```output1
aab

```




```output2
aaaaabacab

```




```output3
ababab

```




```output4
aababacabacabad

```


