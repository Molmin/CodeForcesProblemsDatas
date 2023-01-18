## Description

<div><p>Numbers <span class="tex-span"><i>k</i></span>-bonacci (<span class="tex-span"><i>k</i></span> is integer, <span class="tex-span"><i>k</i> &gt; 1</span>) are a generalization of Fibonacci numbers and are determined as follows:</p><ul> <li> <span class="tex-span"><i>F</i>(<i>k</i>, <i>n</i>) = 0</span>, for integer <span class="tex-span"><i>n</i></span>, <span class="tex-span">1 ≤ <i>n</i> &lt; <i>k</i></span>; </li><li> <span class="tex-span"><i>F</i>(<i>k</i>, <i>k</i>) = 1</span>; </li><li> <span class="tex-span"><i>F</i>(<i>k</i>, <i>n</i>) = <i>F</i>(<i>k</i>, <i>n</i> - 1) + <i>F</i>(<i>k</i>, <i>n</i> - 2) + ... + <i>F</i>(<i>k</i>, <i>n</i> - <i>k</i>)</span>, for integer <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>n</i> &gt; <i>k</i></span>. </li></ul><p>Note that we determine the <span class="tex-span"><i>k</i></span>-bonacci numbers, <span class="tex-span"><i>F</i>(<i>k</i>, <i>n</i>)</span>, only for integer values of <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>.</p><p>You've got a number <span class="tex-span"><i>s</i></span>, represent it as a sum of several (at least two) <span class="tex-font-style-bf">distinct</span> <span class="tex-span"><i>k</i></span>-bonacci numbers. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>s</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>k</i> &gt; 1)</span>.</p></div><div class="output-specification"><p>In the first line print an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> ≥ 2)</span> that shows how many numbers are in the found representation. In the second line print <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>. Each printed integer should be a <span class="tex-span"><i>k</i></span>-bonacci number. The sum of printed integers must equal <span class="tex-span"><i>s</i></span>.</p><p>It is guaranteed that the answer exists. If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>s</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>k</i> &gt; 1)</span>.</p>

## Output

<p>In the first line print an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> ≥ 2)</span> that shows how many numbers are in the found representation. In the second line print <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>. Each printed integer should be a <span class="tex-span"><i>k</i></span>-bonacci number. The sum of printed integers must equal <span class="tex-span"><i>s</i></span>.</p><p>It is guaranteed that the answer exists. If there are several possible answers, print any of them.</p>





```input1
5 2

```




```input2
21 5

```




```output1
3
0 2 3

```




```output2
3
4 1 16

```


