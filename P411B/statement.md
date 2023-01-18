## Description

<div><p>The research center Q has developed a new multi-core processor. The processor consists of <span class="tex-span"><i>n</i></span> cores and has <span class="tex-span"><i>k</i></span> cells of cache memory. Consider the work of this processor.</p><p>At each cycle each core of the processor gets one instruction: either do nothing, or the number of the memory cell (the core will write an information to the cell). After receiving the command, the core executes it immediately. Sometimes it happens that at one cycle, multiple cores try to write the information into a single cell. Unfortunately, the developers did not foresee the possibility of resolving conflicts between cores, so in this case there is a <span class="tex-font-style-it">deadlock</span>: all these cores and the corresponding memory cell are locked forever. Each of the locked cores ignores all further commands, and no core in the future will be able to record an information into the locked cell. If any of the cores tries to write an information into some locked cell, it is immediately locked.</p><p>The development team wants to explore the deadlock situation. Therefore, they need a program that will simulate the processor for a given set of instructions for each core within <span class="tex-span"><i>m</i></span> cycles . You're lucky, this interesting work is entrusted to you. According to the instructions, during the <span class="tex-span"><i>m</i></span> cycles define for each core the number of the cycle, during which it will become locked. It is believed that initially all cores and all memory cells are not locked.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100)</span>. Then follow <span class="tex-span"><i>n</i></span> lines describing instructions. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>1</sub>, <i>x</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>x</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> is the instruction that must be executed by the <span class="tex-span"><i>i</i></span>-th core at the <span class="tex-span"><i>j</i></span>-th cycle. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> equals 0, then the corresponding instruction is «do nothing». But if <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> is a number from 1 to <span class="tex-span"><i>k</i></span>, then the corresponding instruction is «write information to the memory cell number <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span>».</p><p>We assume that the cores are numbered from 1 to <span class="tex-span"><i>n</i></span>, the work cycles are numbered from 1 to <span class="tex-span"><i>m</i></span> and the memory cells are numbered from 1 to <span class="tex-span"><i>k</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. This number should be equal to 0 if the <span class="tex-span"><i>i</i></span>-th core won't be locked, or it should be equal to the number of the cycle when this core will be locked.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100)</span>. Then follow <span class="tex-span"><i>n</i></span> lines describing instructions. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>1</sub>, <i>x</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>x</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> is the instruction that must be executed by the <span class="tex-span"><i>i</i></span>-th core at the <span class="tex-span"><i>j</i></span>-th cycle. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> equals 0, then the corresponding instruction is «do nothing». But if <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span> is a number from 1 to <span class="tex-span"><i>k</i></span>, then the corresponding instruction is «write information to the memory cell number <span class="tex-span"><i>x</i><sub class="lower-index"><i>ij</i></sub></span>».</p><p>We assume that the cores are numbered from 1 to <span class="tex-span"><i>n</i></span>, the work cycles are numbered from 1 to <span class="tex-span"><i>m</i></span> and the memory cells are numbered from 1 to <span class="tex-span"><i>k</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. This number should be equal to 0 if the <span class="tex-span"><i>i</i></span>-th core won't be locked, or it should be equal to the number of the cycle when this core will be locked.</p>





```input1
4 3 5
1 0 0
1 0 2
2 3 1
3 2 0

```




```input2
3 2 2
1 2
1 2
2 2

```




```input3
1 1 1
0

```




```output1
1
1
3
0

```




```output2
1
1
0

```




```output3
0

```


