## Description

<div><p>There are <span class="tex-span"><i>n</i></span> children in Jzzhu's school. Jzzhu is going to give some candies to them. Let's number all the children from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th child wants to get at least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> candies.</p><p>Jzzhu asks children to line up. Initially, the <span class="tex-span"><i>i</i></span>-th child stands at the <span class="tex-span"><i>i</i></span>-th place of the line. Then Jzzhu start distribution of the candies. He follows the algorithm:</p><ol> <li> Give <span class="tex-span"><i>m</i></span> candies to the first child of the line. </li><li> If this child still haven't got enough candies, then the child goes to the end of the line, else the child go home. </li><li> Repeat the first two steps while the line is not empty. </li></ol><p>Consider all the children in the order they go home. Jzzhu wants to know, which child will be the last in this order?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>m</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p></div><div class="output-specification"><p>Output a single integer, representing the number of the last child.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>m</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p>

## Output

<p>Output a single integer, representing the number of the last child.</p>





```input1
5 2
1 3 1 4 2

```




```input2
6 4
1 1 2 2 3 3

```




```output1
4

```




```output2
6

```



## Note

<p>Let's consider the first sample. </p><p>Firstly child 1 gets 2 candies and go home. Then child 2 gets 2 candies and go to the end of the line. Currently the line looks like [3, 4, 5, 2] (indices of the children in order of the line). Then child 3 gets 2 candies and go home, and then child 4 gets 2 candies and goes to the end of the line. Currently the line looks like [5, 2, 4]. Then child 5 gets 2 candies and goes home. Then child 2 gets two candies and goes home, and finally child 4 gets 2 candies and goes home.</p><p>Child 4 is the last one who goes home.</p>
