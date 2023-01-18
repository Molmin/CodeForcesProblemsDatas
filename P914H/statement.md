## Description

<div><p>Ember and Storm play a game. First, Ember picks a labelled tree <span class="tex-span"><i>T</i></span> of <span class="tex-span"><i>n</i></span> vertices, such that the degree of every vertex is at most <span class="tex-span"><i>d</i></span>. Then, Storm picks two distinct vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> in this tree and writes down the labels of the vertices in the path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> in a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>k</i></sub></span>. Finally, Ember picks any index <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>) in the array. Now he performs one of the following two operations exactly once:</p><ul> <li> flip the subrange <span class="tex-span">[<i>i</i> + 1, <i>k</i>]</span> and add <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to it. After this, the sequence becomes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ... <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>k</i></sub> + <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>k</i> - 1</sub> + <i>a</i><sub class="lower-index"><i>i</i></sub>, ... <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> + <i>a</i><sub class="lower-index"><i>i</i></sub></span> </li><li> negate the subrange <span class="tex-span">[<i>i</i> + 1, <i>k</i>]</span> and add <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to it. i.e., the array becomes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ... <i>a</i><sub class="lower-index"><i>i</i></sub>,  - <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> + <i>a</i><sub class="lower-index"><i>i</i></sub>,  - <i>a</i><sub class="lower-index"><i>i</i> + 2</sub> + <i>a</i><sub class="lower-index"><i>i</i></sub>, ... - <i>a</i><sub class="lower-index"><i>k</i></sub> + <i>a</i><sub class="lower-index"><i>i</i></sub></span> </li></ul><p>Ember wins if the array is monotonically increasing or decreasing after this. Otherwise Storm wins.</p><p>The game can be described by the tuple <span class="tex-span">(<i>T</i>, <i>u</i>, <i>v</i>, <i>i</i>, <i>op</i>)</span> where <span class="tex-span"><i>op</i></span> is «flip» or «negate» depending on the action Ember chose in the last turn. Find the number of tuples that can occur if Ember and Storm play optimally. When they play optimally, if there are multiple moves by which they are guaranteed to win, then they may play any of the winning moves. Otherwise, if someone loses no matter what they play, then they may play any of the possible moves.</p><p>Report the answer modulo <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The input consists of a single line containing three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200, 1 ≤ <i>d</i> &lt; <i>n</i>, 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single number &nbsp;— the number of possible tuples if Ember and Storm play as described, modulo <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The input consists of a single line containing three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200, 1 ≤ <i>d</i> &lt; <i>n</i>, 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single number &nbsp;— the number of possible tuples if Ember and Storm play as described, modulo <span class="tex-span"><i>m</i></span>.</p>





```input1
2 1 1000000007

```




```input2
3 1 250

```




```input3
3 2 100

```




```output1
4

```




```output2
0

```




```output3
36

```



## Note

<p>In the first sample case, there is only one possible tree. There are two possible paths, <span class="tex-span">1</span> to <span class="tex-span">2</span> and <span class="tex-span">2</span> to <span class="tex-span">1</span>. For both paths, <span class="tex-span"><i>i</i></span> can only be <span class="tex-span">1</span>, and <span class="tex-span"><i>op</i></span> can take both possibilities. Therefore, the answer is <span class="tex-span">4</span>.</p><p>In the second sample, there are no possible trees.</p><p>In the third sample, there are three possible trees. </p>
