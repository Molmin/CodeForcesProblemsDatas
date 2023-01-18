## Description

<div><p>Dima's got a staircase that consists of <span class="tex-span"><i>n</i></span> stairs. The first stair is at height <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, the second one is at <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, the last one is at <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>). </p><p>Dima decided to play with the staircase, so he is throwing rectangular boxes at the staircase from above. The <span class="tex-span"><i>i</i></span>-th box has width <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Dima throws each box vertically down on the first <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> stairs of the staircase, that is, the box covers stairs with numbers <span class="tex-span">1, 2, ..., <i>w</i><sub class="lower-index"><i>i</i></sub></span>. Each thrown box flies vertically down until at least one of the two following events happen:</p><ul> <li> the bottom of the box touches the top of a stair; </li><li> the bottom of the box touches the top of a box, thrown earlier. </li></ul><p>We only consider touching of the horizontal sides of stairs and boxes, at that touching with the corners isn't taken into consideration. Specifically, that implies that a box with width <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> cannot touch the stair number <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub> + 1</span>.</p><p>You are given the description of the staircase and the sequence in which Dima threw the boxes at it. For each box, determine how high the bottom of the box after landing will be. Consider a box to fall after the previous one lands.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stairs in the staircase. The second line contains a non-decreasing sequence, consisting of <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of boxes. Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the size of the <span class="tex-span"><i>i</i></span>-th thrown box.</p><p>The numbers in the lines are separated by spaces.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — for each box the height, where the bottom of the box will be after landing. Print the answers for the boxes in the order, in which the boxes are given in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stairs in the staircase. The second line contains a non-decreasing sequence, consisting of <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of boxes. Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the size of the <span class="tex-span"><i>i</i></span>-th thrown box.</p><p>The numbers in the lines are separated by spaces.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — for each box the height, where the bottom of the box will be after landing. Print the answers for the boxes in the order, in which the boxes are given in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
1 2 3 6 6
4
1 1
3 1
1 1
4 3

```




```input2
3
1 2 3
2
1 1
3 1

```




```input3
1
1
5
1 2
1 10
1 10
1 10
1 10

```




```output1
1
3
4
6

```




```output2
1
3

```




```output3
1
3
13
23
33

```



## Note

<p>The first sample are shown on the picture.</p><center> <img class="tex-graphics" src="file://si3ZkuGV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
