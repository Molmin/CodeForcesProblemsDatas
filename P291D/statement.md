## Description

<div><p>Polycarpus has a computer with <span class="tex-span"><i>n</i></span> processors. Also, his computer has <span class="tex-span"><i>n</i></span> memory cells. We'll consider the processors numbered by integers from 1 to <span class="tex-span"><i>n</i></span> and that the memory cells are consecutively numbered by integers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>Polycarpus needs to come up with a parallel program model. For each memory cell number <span class="tex-span"><i>i</i></span> this program must record the value <span class="tex-span"><i>n</i> - <i>i</i></span> to this cell. In other words, for each cell you've got to find the distance to cell <span class="tex-span"><i>n</i></span>.</p><p>Let's denote the value that is written in the <span class="tex-span"><i>i</i></span>-th cell as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Initially, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 0</span>. We will consider that only processor <span class="tex-span"><i>i</i></span> can write values in the memory cell number <span class="tex-span"><i>i</i></span>. All processors can read an information from some cell (several processors can read an information from some cell simultaneously).</p><p>The parallel program is executed in several steps. During each step we execute the <span class="tex-font-style-it">parallel version of the increment operation</span>. Executing the parallel version of the increment operation goes as follows:</p><ol> <li> Each processor independently of the other ones chooses some memory cell. Let's say that processor <span class="tex-span"><i>i</i></span> has chosen a cell with number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. </li><li> All processors <span class="tex-font-style-it">simultaneously</span> execute operation <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i></sub></sub></span>. </li></ol><p>Help Polycarpus come up with the parallel program model that is executed in exactly <span class="tex-span"><i>k</i></span> steps. Calculate the operations that need to be executed. Note that after <span class="tex-span"><i>k</i></span> steps for all <span class="tex-span"><i>i</i></span>'s value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must be equal <span class="tex-span"><i>n</i> - <i>i</i></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i> ≤ 20)</span>.</p><p>It is guaranteed that at the given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> the required sequence of operations exists.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>n</i>·<i>k</i></span> integers in <span class="tex-span"><i>k</i></span> lines. In the first line print numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> for the first increment operation. In the second line print the numbers for the second increment operation. In the <span class="tex-span"><i>k</i></span>-th line print the numbers for the <span class="tex-span"><i>k</i></span>-th increment operation.</p><p>As a result of the printed operations for any <span class="tex-span"><i>i</i></span> value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must equal <span class="tex-span"><i>n</i> - <i>i</i></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i> ≤ 20)</span>.</p><p>It is guaranteed that at the given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> the required sequence of operations exists.</p>

## Output

<p>Print exactly <span class="tex-span"><i>n</i>·<i>k</i></span> integers in <span class="tex-span"><i>k</i></span> lines. In the first line print numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> for the first increment operation. In the second line print the numbers for the second increment operation. In the <span class="tex-span"><i>k</i></span>-th line print the numbers for the <span class="tex-span"><i>k</i></span>-th increment operation.</p><p>As a result of the printed operations for any <span class="tex-span"><i>i</i></span> value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> must equal <span class="tex-span"><i>n</i> - <i>i</i></span>.</p>





```input1
1 1

```




```input2
3 2

```




```output1
1

```




```output2
2 3 3
3 3 3

```


