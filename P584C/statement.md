## Description

<div><p>Marina loves strings of the same length and Vasya loves when there is a third string, different from them in exactly <span class="tex-span"><i>t</i></span> characters. Help Vasya find at least one such string.</p><p>More formally, you are given two strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> of length <span class="tex-span"><i>n</i></span> and number <span class="tex-span"><i>t</i></span>. Let's denote as <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>)</span> the number of characters in which strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are different. Then your task will be to find any string <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> of length <span class="tex-span"><i>n</i></span>, such that <span class="tex-span"><i>f</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">3</sub>) = <i>f</i>(<i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>) = <i>t</i></span>. If there is no such string, print <span class="tex-span"> - 1</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p><p>The third line contain string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print a string of length <span class="tex-span"><i>n</i></span>, differing from string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and from <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> in exactly <span class="tex-span"><i>t</i></span> characters. Your string should consist only from lowercase English letters. If such string doesn't exist, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>t</i> ≤ <i>n</i></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p><p>The third line contain string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p>

## Output

<p>Print a string of length <span class="tex-span"><i>n</i></span>, differing from string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and from <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> in exactly <span class="tex-span"><i>t</i></span> characters. Your string should consist only from lowercase English letters. If such string doesn't exist, print -1.</p>





```input1
3 2
abc
xyc

```




```input2
1 0
c
b

```




```output1
ayd
```




```output2
-1

```


