## Description

<div><p>Fox Ciel is in the Amusement Park. And now she is in a queue in front of the Ferris wheel. There are <span class="tex-span"><i>n</i></span> people (or foxes more precisely) in the queue: we use first people to refer one at the head of the queue, and <span class="tex-span"><i>n</i></span>-th people to refer the last one in the queue.</p><p>There will be <span class="tex-span"><i>k</i></span> gondolas, and the way we allocate gondolas looks like this:</p><ul> <li> When the first gondolas come, the <span class="tex-span"><i>q</i><sub class="lower-index">1</sub></span> people in head of the queue go into the gondolas. </li><li> Then when the second gondolas come, the <span class="tex-span"><i>q</i><sub class="lower-index">2</sub></span> people in head of the remain queue go into the gondolas.<p>&nbsp;&nbsp;&nbsp;&nbsp;...</p></li><li> The remain <span class="tex-span"><i>q</i><sub class="lower-index"><i>k</i></sub></span> people go into the last (<span class="tex-span"><i>k</i></span>-th) gondolas. </li></ul><p>Note that <span class="tex-span"><i>q</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>q</i><sub class="lower-index"><i>k</i></sub></span> must be positive. You can get from the statement that <img align="middle" class="tex-formula" src="file://lpC0RupF.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span>.</p><p>You know, people don't want to stay with strangers in the gondolas, so your task is to find an optimal allocation way (that is find an optimal sequence <span class="tex-span"><i>q</i></span>) to make people happy. For every pair of people <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, there exists a value <span class="tex-span"><i>u</i><sub class="lower-index"><i>ij</i></sub></span> denotes a level of unfamiliar. You can assume <span class="tex-span"><i>u</i><sub class="lower-index"><i>ij</i></sub> = <i>u</i><sub class="lower-index"><i>ji</i></sub></span> for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>ii</i></sub> = 0</span> for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>. Then an unfamiliar value of a gondolas is the sum of the levels of unfamiliar between any pair of people that is into the gondolas.</p><p>A total unfamiliar value is the sum of unfamiliar values for all gondolas. Help Fox Ciel to find the minimal possible total unfamiliar value for some optimal allocation.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 800)</span>) — the number of people in the queue and the number of gondolas. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers — matrix <span class="tex-span"><i>u</i></span>, (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>ij</i></sub> ≤ 9</span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>ij</i></sub> = <i>u</i><sub class="lower-index"><i>ji</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>ii</i></sub> = 0</span>).</p><p>Please, use fast input methods (for example, please use BufferedReader instead of Scanner for Java).</p></div><div class="output-specification"><p>Print an integer — the minimal possible total unfamiliar value.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 800)</span>) — the number of people in the queue and the number of gondolas. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers — matrix <span class="tex-span"><i>u</i></span>, (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>ij</i></sub> ≤ 9</span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>ij</i></sub> = <i>u</i><sub class="lower-index"><i>ji</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>ii</i></sub> = 0</span>).</p><p>Please, use fast input methods (for example, please use BufferedReader instead of Scanner for Java).</p>

## Output

<p>Print an integer — the minimal possible total unfamiliar value.</p>





```input1
5 2
0 0 1 1 1
0 0 1 1 1
1 1 0 0 0
1 1 0 0 0
1 1 0 0 0

```




```input2
8 3
0 1 1 1 1 1 1 1
1 0 1 1 1 1 1 1
1 1 0 1 1 1 1 1
1 1 1 0 1 1 1 1
1 1 1 1 0 1 1 1
1 1 1 1 1 0 1 1
1 1 1 1 1 1 0 1
1 1 1 1 1 1 1 0

```




```input3
3 2
0 2 0
2 0 3
0 3 0

```




```output1
0

```




```output2
7

```




```output3
2

```



## Note

<p>In the first example, we can allocate people like this: {1, 2} goes into a gondolas, {3, 4, 5} goes into another gondolas.</p><p>In the second example, an optimal solution is : {1, 2, 3} | {4, 5, 6} | {7, 8}.</p>
