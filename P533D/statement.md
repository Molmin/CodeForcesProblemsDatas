## Description

<div><p>We have an old building with <span class="tex-span"><i>n</i> + 2</span> columns in a row. These columns support the ceiling. These columns are located in points with coordinates <span class="tex-span">0 = <i>x</i><sub class="lower-index">0</sub> &lt; <i>x</i><sub class="lower-index">1</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i></sub> &lt; <i>x</i><sub class="lower-index"><i>n</i> + 1</sub></span>. The leftmost and the rightmost columns are special, we will call them <span class="tex-font-style-it">bearing</span>, the other columns are <span class="tex-font-style-it">ordinary</span>. </p><p>For each column we know its durability <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Let's consider an ordinary column with coordinate <span class="tex-span"><i>x</i></span>. Let's assume that the coordinate of the closest to it column to the left (bearing or ordinary) is <span class="tex-span"><i>a</i></span> and the coordinate of the closest to it column to the right (also, bearing or ordinary) is <span class="tex-span"><i>b</i></span>. In this task let's assume that this column supports the segment of the ceiling from point <img align="middle" class="tex-formula" src="file://KvsPYnNG.png" style="max-width: 100.0%;max-height: 100.0%;"> to point <img align="middle" class="tex-formula" src="file://oDXUfVLp.png" style="max-width: 100.0%;max-height: 100.0%;"> (here both fractions are considered as real division). If the length of the segment of the ceiling supported by the column exceeds <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, then the column cannot support it and it crashes after a while, and after that the load is being redistributeed between the neighbouring columns according to the same principle.</p><center> <img class="tex-graphics" src="file://PsFrOQ63.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Thus, ordinary columns will be crashing for some time until the process stops at some state. One can prove that the set of the remaining columns doesn't depend on the order in which columns crash. If there are only two bearing columns left in the end, then we assume that the whole construction crashes under the weight of the roof. But if at least one ordinary column stays in addition to the bearing ones, then the building doesn't crash.</p><p>To make the building stronger, we can add one extra ordinary column of arbitrary durability <span class="tex-span"><i>d</i>'</span> at any (not necessarily integer) point <span class="tex-span">0 &lt; <i>x</i>' &lt; <i>x</i><sub class="lower-index"><i>n</i> + 1</sub></span>. If point <span class="tex-span"><i>x</i>'</span> is already occupied by an ordinary column, it is replaced by a new one.</p><p>Your task is to find out: what minimal durability can the added column have so that the building doesn't crash?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of ordinary columns.</p><p>The second line contains <span class="tex-span"><i>n</i> + 2</span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>, <i>x</i><sub class="lower-index"><i>n</i> + 1</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index">0</sub> = 0</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i> + 1</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the columns.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single number — the minimum possible durability of the column that you need to add in order to make the building stay. If you do not have to add the column, please print <span class="tex-span">0</span>. Your answer will be checked with the relative or absolute error <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of ordinary columns.</p><p>The second line contains <span class="tex-span"><i>n</i> + 2</span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub>, <i>x</i><sub class="lower-index"><i>n</i> + 1</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index">0</sub> = 0</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i> + 1</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the columns.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single number — the minimum possible durability of the column that you need to add in order to make the building stay. If you do not have to add the column, please print <span class="tex-span">0</span>. Your answer will be checked with the relative or absolute error <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
2
0 20 40 100
15 40

```




```input2
3
0 4 10 28 30
9 13 5

```




```output1
10

```




```output2
0

```


