## Description

<div><p>Consider a sequence <span class="tex-span">[<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub>]</span>. Define its prefix product sequence <img align="middle" class="tex-formula" src="file://F5Mu1Tae.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Now given <span class="tex-span"><i>n</i></span>, find a permutation of <span class="tex-span">[1, 2, ..., <i>n</i>]</span>, such that its prefix product sequence is a permutation of <span class="tex-span">[0, 1, ..., <i>n</i> - 1]</span>.</p></div><div class="input-specification"><p>The only input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>In the first output line, print "<span class="tex-font-style-tt">YES</span>" if such sequence exists, or print "<span class="tex-font-style-tt">NO</span>" if no such sequence exists.</p><p>If any solution exists, you should output <span class="tex-span"><i>n</i></span> more lines. <span class="tex-span"><i>i</i></span>-th line contains only an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The elements of the sequence should be different positive integers no larger than <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple solutions, you are allowed to print any of them.</p></div>

## Input

<p>The only input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>In the first output line, print "<span class="tex-font-style-tt">YES</span>" if such sequence exists, or print "<span class="tex-font-style-tt">NO</span>" if no such sequence exists.</p><p>If any solution exists, you should output <span class="tex-span"><i>n</i></span> more lines. <span class="tex-span"><i>i</i></span>-th line contains only an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The elements of the sequence should be different positive integers no larger than <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple solutions, you are allowed to print any of them.</p>





```input1
7

```




```input2
6

```




```output1
YES
1
4
3
6
5
2
7

```




```output2
NO

```



## Note

<p>For the second sample, there are no valid sequences.</p>
