## Description

<div><p>On Children's Day, the child got a toy from Delayyy as a present. However, the child is so naughty that he can't wait to destroy the toy.</p><p>The toy consists of <span class="tex-span"><i>n</i></span> parts and <span class="tex-span"><i>m</i></span> ropes. Each rope links two parts, but every pair of parts is linked by at most one rope. To split the toy, the child must remove all its parts. The child can remove a single part at a time, and each remove consume an energy. Let's define an energy value of part <span class="tex-span"><i>i</i></span> as <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. The child spend <span class="tex-span"><i>v</i><sub class="lower-index"><i>f</i><sub class="lower-index">1</sub></sub> + <i>v</i><sub class="lower-index"><i>f</i><sub class="lower-index">2</sub></sub> + ... + <i>v</i><sub class="lower-index"><i>f</i><sub class="lower-index"><i>k</i></sub></sub></span> energy for removing part <span class="tex-span"><i>i</i></span> where <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>k</i></sub></span> are the parts that are directly connected to the <span class="tex-span"><i>i</i></span>-th and haven't been removed.</p><p>Help the child to find out, what is the minimum total energy he should spend to remove all <span class="tex-span"><i>n</i></span> parts.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then followed <span class="tex-span"><i>m</i></span> lines, each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, representing a rope from part <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to part <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Consider all the parts are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Output the minimum total energy the child should spend to remove all <span class="tex-span"><i>n</i></span> parts of the toy.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then followed <span class="tex-span"><i>m</i></span> lines, each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, representing a rope from part <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to part <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Consider all the parts are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Output the minimum total energy the child should spend to remove all <span class="tex-span"><i>n</i></span> parts of the toy.</p>





```input1
4 3
10 20 30 40
1 4
1 2
2 3

```




```input2
4 4
100 100 100 100
1 2
2 3
2 4
3 4

```




```input3
7 10
40 10 20 10 20 80 40
1 5
4 7
4 5
5 2
5 7
6 4
1 6
1 3
4 3
1 4

```




```output1
40

```




```output2
400

```




```output3
160

```



## Note

<p>One of the optimal sequence of actions in the first sample is:</p><ul> <li> First, remove part <span class="tex-span">3</span>, cost of the action is <span class="tex-span">20</span>. </li><li> Then, remove part <span class="tex-span">2</span>, cost of the action is <span class="tex-span">10</span>. </li><li> Next, remove part <span class="tex-span">4</span>, cost of the action is <span class="tex-span">10</span>. </li><li> At last, remove part <span class="tex-span">1</span>, cost of the action is <span class="tex-span">0</span>. </li></ul><p>So the total energy the child paid is <span class="tex-span">20 + 10 + 10 + 0 = 40</span>, which is the minimum.</p><p>In the second sample, the child will spend <span class="tex-span">400</span> no matter in what order he will remove the parts.</p>
