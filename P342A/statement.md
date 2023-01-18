## Description

<div><p>Xenia the mathematician has a sequence consisting of <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i></span> is divisible by 3) positive integers, each of them is at most 7. She wants to split the sequence into groups of three so that for each group of three <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> the following conditions held:</p><ul> <li> <span class="tex-span"><i>a</i> &lt; <i>b</i> &lt; <i>c</i></span>; </li><li> <span class="tex-span"><i>a</i></span> divides <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>b</i></span> divides <span class="tex-span"><i>c</i></span>. </li></ul><p>Naturally, Xenia wants each element of the sequence to belong to exactly one group of three. Thus, if the required partition exists, then it has <img align="middle" class="tex-formula" src="file://8ISUciCP.png" style="max-width: 100.0%;max-height: 100.0%;"> groups of three.</p><p>Help Xenia, find the required partition or else say that it doesn't exist.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 99999)</span> — the number of elements in the sequence. The next line contains <span class="tex-span"><i>n</i></span> positive integers, each of them is at most 7.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by 3.</p></div><div class="output-specification"><p>If the required partition exists, print <img align="middle" class="tex-formula" src="file://37XYjQmj.png" style="max-width: 100.0%;max-height: 100.0%;"> groups of three. Print each group as values of the elements it contains. You should print values in increasing order. Separate the groups and integers in groups by whitespaces. If there are multiple solutions, you can print any of them.</p><p>If there is no solution, print -1.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 99999)</span> — the number of elements in the sequence. The next line contains <span class="tex-span"><i>n</i></span> positive integers, each of them is at most 7.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by 3.</p>

## Output

<p>If the required partition exists, print <img align="middle" class="tex-formula" src="file://37XYjQmj.png" style="max-width: 100.0%;max-height: 100.0%;"> groups of three. Print each group as values of the elements it contains. You should print values in increasing order. Separate the groups and integers in groups by whitespaces. If there are multiple solutions, you can print any of them.</p><p>If there is no solution, print -1.</p>





```input1
6
1 1 1 2 2 2

```




```input2
6
2 2 1 1 4 6

```




```output1
-1

```




```output2
1 2 4
1 2 6

```


