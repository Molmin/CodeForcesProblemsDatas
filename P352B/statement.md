## Description

<div><p>One day Jeff got hold of an integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>. The boy immediately decided to analyze the sequence. For that, he needs to find all values of <span class="tex-span"><i>x</i></span>, for which these conditions hold:</p><ul> <li> <span class="tex-span"><i>x</i></span> occurs in sequence <span class="tex-span"><i>a</i></span>. </li><li> Consider all positions of numbers <span class="tex-span"><i>x</i></span> in the sequence <span class="tex-span"><i>a</i></span> (such <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>x</i></span>). These numbers, sorted in the increasing order, must form an arithmetic progression. </li></ul><p>Help Jeff, find all <span class="tex-span"><i>x</i></span> that meet the problem conditions.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The numbers are separated by spaces.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>t</i></span> — the number of valid <span class="tex-span"><i>x</i></span>. On each of the next <span class="tex-span"><i>t</i></span> lines print two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span>, where <span class="tex-span"><i>x</i></span> is current suitable value, <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> is the common difference between numbers in the progression (if <span class="tex-span"><i>x</i></span> occurs exactly once in the sequence, <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> must equal 0). Print the pairs in the order of increasing <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The numbers are separated by spaces.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>t</i></span> — the number of valid <span class="tex-span"><i>x</i></span>. On each of the next <span class="tex-span"><i>t</i></span> lines print two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span>, where <span class="tex-span"><i>x</i></span> is current suitable value, <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> is the common difference between numbers in the progression (if <span class="tex-span"><i>x</i></span> occurs exactly once in the sequence, <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> must equal 0). Print the pairs in the order of increasing <span class="tex-span"><i>x</i></span>.</p>





```input1
1
2

```




```input2
8
1 2 1 3 1 2 1 5

```




```output1
1
2 0

```




```output2
4
1 2
2 4
3 0
5 0

```



## Note

<p>In the first test <span class="tex-span">2</span> occurs exactly once in the sequence, ergo <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = 0</span>.</p>
