## Description

<div><p>Programmers working on a large project have just received a task to write exactly <span class="tex-span"><i>m</i></span> lines of code. There are <span class="tex-span"><i>n</i></span> programmers working on a project, the <span class="tex-span"><i>i</i></span>-th of them makes exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bugs in every line of code that he writes. </p><p>Let's call a sequence of non-negative integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> a <span class="tex-font-style-it">plan</span>, if <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> + <i>v</i><sub class="lower-index">2</sub> + ... + <i>v</i><sub class="lower-index"><i>n</i></sub> = <i>m</i></span>. The programmers follow the plan like that: in the beginning the first programmer writes the first <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> lines of the given task, then the second programmer writes <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> more lines of the given task, and so on. In the end, the last programmer writes the remaining lines of the code. Let's call a plan <span class="tex-font-style-it">good</span>, if all the written lines of the task contain at most <span class="tex-span"><i>b</i></span> bugs in total.</p><p>Your task is to determine how many distinct <span class="tex-font-style-it">good</span> plans are there. As the number of plans can be large, print the remainder of this number modulo given positive integer <span class="tex-span"><i>mod</i></span>.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 500</span>; <span class="tex-span">1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>)&nbsp;— the number of programmers, the number of lines of code in the task, the maximum total number of bugs respectively and the modulo you should use when printing the answer.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the number of bugs per line for each programmer.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span"><i>mod</i></span>.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 500</span>; <span class="tex-span">1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>)&nbsp;— the number of programmers, the number of lines of code in the task, the maximum total number of bugs respectively and the modulo you should use when printing the answer.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the number of bugs per line for each programmer.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span"><i>mod</i></span>.</p>





```input1
3 3 3 100
1 1 1

```




```input2
3 6 5 1000000007
1 2 3

```




```input3
3 5 6 11
1 2 1

```




```output1
10

```




```output2
0

```




```output3
0

```


