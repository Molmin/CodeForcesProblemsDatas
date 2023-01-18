## Description

<div><p>Mishka has got <span class="tex-span"><i>n</i></span> empty boxes. For every <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), <span class="tex-span"><i>i</i></span>-th box is a cube with side length <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Mishka can put a box <span class="tex-span"><i>i</i></span> into another box <span class="tex-span"><i>j</i></span> if the following conditions are met:</p><ul> <li> <span class="tex-span"><i>i</i></span>-th box is not put into another box; </li><li> <span class="tex-span"><i>j</i></span>-th box doesn't contain any other boxes; </li><li> box <span class="tex-span"><i>i</i></span> is smaller than box <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>). </li></ul><p>Mishka can put boxes into each other an arbitrary number of times. He wants to minimize the number of <span class="tex-font-style-it">visible</span> boxes. A box is called <span class="tex-font-style-it">visible</span> iff it is not put into some another box.</p><p>Help Mishka to determine the minimum possible number of <span class="tex-font-style-it">visible</span> boxes!</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of boxes Mishka has got.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the side length of <span class="tex-span"><i>i</i></span>-th box.</p></div><div class="output-specification"><p>Print the minimum possible number of <span class="tex-font-style-it">visible</span> boxes.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of boxes Mishka has got.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the side length of <span class="tex-span"><i>i</i></span>-th box.</p>

## Output

<p>Print the minimum possible number of <span class="tex-font-style-it">visible</span> boxes.</p>





```input1
3
1 2 3

```




```input2
4
4 2 4 3

```




```output1
1

```




```output2
2

```



## Note

<p>In the first example it is possible to put box <span class="tex-span">1</span> into box <span class="tex-span">2</span>, and <span class="tex-span">2</span> into <span class="tex-span">3</span>.</p><p>In the second example Mishka can put box <span class="tex-span">2</span> into box <span class="tex-span">3</span>, and box <span class="tex-span">4</span> into box <span class="tex-span">1</span>.</p>
