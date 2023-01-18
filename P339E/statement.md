## Description

<div><p>Xenia the horse breeder has <span class="tex-span"><i>n</i></span> <span class="tex-span">(<i>n</i> &gt; 1)</span> horses that stand in a row. Each horse has its own unique number. Initially, the <span class="tex-span"><i>i</i></span>-th left horse has number <span class="tex-span"><i>i</i></span>. That is, the sequence of numbers of horses in a row looks as follows (from left to right): 1, 2, 3, <span class="tex-span">...</span>, <span class="tex-span"><i>n</i></span>.</p><p>Xenia trains horses before the performance. During the practice sessions, she consistently gives them commands. Each command is a pair of numbers <span class="tex-span"><i>l</i>, <i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i>)</span>. The command <span class="tex-span"><i>l</i>, <i>r</i></span> means that the horses that are on the <span class="tex-span"><i>l</i></span>-th, <span class="tex-span">(<i>l</i> + 1)</span>-th, <span class="tex-span">(<i>l</i> + 2)</span>-th, <span class="tex-span">...</span>, <span class="tex-span"><i>r</i></span>-th places from the left must be rearranged. The horses that initially stand on the <span class="tex-span"><i>l</i></span>-th and <span class="tex-span"><i>r</i></span>-th places will swap. The horses on the <span class="tex-span">(<i>l</i> + 1)</span>-th and <span class="tex-span">(<i>r</i> - 1)</span>-th places will swap. The horses on the <span class="tex-span">(<i>l</i> + 2)</span>-th and <span class="tex-span">(<i>r</i> - 2)</span>-th places will swap and so on. In other words, the horses that were on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> change their order to the reverse one.</p><p>For example, if Xenia commanded <span class="tex-span"><i>l</i> = 2, <i>r</i> = 5</span>, and the sequence of numbers of horses before the command looked as (2, 1, 3, 4, 5, 6), then after the command the sequence will be (2, 5, 4, 3, 1, 6).</p><p>We know that during the practice Xenia gave at most three commands of the described form. You have got the final sequence of numbers of horses by the end of the practice. Find what commands Xenia gave during the practice. Note that you do not need to minimize the number of commands in the solution, find any valid sequence of at most three commands.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of horses in the row. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the <span class="tex-span"><i>i</i></span>-th left horse in the row after the practice.</p></div><div class="output-specification"><p>The first line should contain integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 3)</span> — the number of commads Xenia gave during the practice. In each of the next <span class="tex-span"><i>k</i></span> lines print two integers. In the <span class="tex-span"><i>i</i></span>-th line print numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — Xenia's <span class="tex-span"><i>i</i></span>-th command during the practice.</p><p>It is guaranteed that a solution exists. If there are several solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of horses in the row. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the <span class="tex-span"><i>i</i></span>-th left horse in the row after the practice.</p>

## Output

<p>The first line should contain integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 3)</span> — the number of commads Xenia gave during the practice. In each of the next <span class="tex-span"><i>k</i></span> lines print two integers. In the <span class="tex-span"><i>i</i></span>-th line print numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — Xenia's <span class="tex-span"><i>i</i></span>-th command during the practice.</p><p>It is guaranteed that a solution exists. If there are several solutions, you are allowed to print any of them.</p>





```input1
5
1 4 3 2 5

```




```input2
6
2 1 4 3 6 5

```




```output1
1
2 4

```




```output2
3
1 2
3 4
5 6

```


