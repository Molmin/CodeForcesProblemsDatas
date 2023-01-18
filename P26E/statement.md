## Description

<div><p>You are given the following concurrent program. There are <span class="tex-span"><i>N</i></span> processes and the <span class="tex-span"><i>i</i></span>-th process has the following pseudocode: </p><pre class="verbatim">repeat <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> times<br>    <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> := <span class="tex-span"><i>y</i></span><br>    <span class="tex-span"><i>y</i></span> := <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> + 1</span><br>end repeat<br></pre><p>Here <span class="tex-span"><i>y</i></span> is a shared variable. Everything else is local for the process. All actions on a given row are atomic, i.e. when the process starts executing a row it is never interrupted. Beyond that all interleavings are possible, i.e. every process that has yet work to do can be granted the rights to execute its next row. In the beginning <span class="tex-span"><i>y</i> = 0</span>. You will be given an integer <span class="tex-span"><i>W</i></span> and <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>, for <span class="tex-span"><i>i</i> = 1, ... , <i>N</i></span>. Determine if it is possible that after all processes terminate, <span class="tex-span"><i>y</i> = <i>W</i></span>, and if it is possible output an arbitrary schedule that will produce this final value.</p></div><div class="input-specification"><p>In the first line of the input you will be given two space separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>) and <span class="tex-span"><i>W</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>). In the second line there are <span class="tex-span"><i>N</i></span> space separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>On the first line of the output write <span class="tex-font-style-tt">Yes</span> if it is possible that at the end <span class="tex-span"><i>y</i> = <i>W</i></span>, or <span class="tex-font-style-tt">No</span> otherwise. If the answer is <span class="tex-font-style-tt">No</span> then there is no second line, but if the answer is <span class="tex-font-style-tt">Yes</span>, then on the second line output a space separated list of integers representing some schedule that leads to the desired result. For more information see note.</p></div>

## Input

<p>In the first line of the input you will be given two space separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>) and <span class="tex-span"><i>W</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>). In the second line there are <span class="tex-span"><i>N</i></span> space separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>On the first line of the output write <span class="tex-font-style-tt">Yes</span> if it is possible that at the end <span class="tex-span"><i>y</i> = <i>W</i></span>, or <span class="tex-font-style-tt">No</span> otherwise. If the answer is <span class="tex-font-style-tt">No</span> then there is no second line, but if the answer is <span class="tex-font-style-tt">Yes</span>, then on the second line output a space separated list of integers representing some schedule that leads to the desired result. For more information see note.</p>





```input1
1 10
11

```




```input2
2 3
4 4

```




```input3
3 6
1 2 3

```




```output1
No

```




```output2
Yes
1 1 2 1 2 2 2 2 2 1 2 1 1 1 1 2

```




```output3
Yes
1 1 2 2 2 2 3 3 3 3 3 3

```



## Note

<p>For simplicity, assume that there is no repeat statement in the code of the processes, but the code from the loop is written the correct amount of times. The processes are numbered starting from 1. The list of integers represent which process works on its next instruction at a given step. For example, consider the schedule <span class="tex-font-style-tt">1 2 2 1 3</span>. First process <span class="tex-font-style-tt">1</span> executes its first instruction, then process <span class="tex-font-style-tt">2</span> executes its first two instructions, after that process <span class="tex-font-style-tt">1</span> executes its second instruction, and finally process <span class="tex-font-style-tt">3</span> executes its first instruction. The list must consists of exactly <span class="tex-span">2·Σ <sub class="lower-index"><i>i</i> = 1...<i>N</i></sub> <i>n</i><sub class="lower-index"><i>i</i></sub></span> numbers.</p>
