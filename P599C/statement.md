## Description

<div><p>One day Squidward, Spongebob and Patrick decided to go to the beach. Unfortunately, the weather was bad, so the friends were unable to ride waves. However, they decided to spent their time building sand castles.</p><p>At the end of the day there were <span class="tex-span"><i>n</i></span> castles built by friends. Castles are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the height of the <span class="tex-span"><i>i</i></span>-th castle is equal to <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. When friends were about to leave, Squidward noticed, that castles are not ordered by their height, and this looks ugly. Now friends are going to reorder the castles in a way to obtain that condition <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i><sub class="lower-index"><i>i</i> + 1</sub></span> holds for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span>.</p><p>Squidward suggested the following process of sorting castles: </p><ul> <li> Castles are split into <span class="tex-font-style-it">blocks</span>&nbsp;— groups of <span class="tex-font-style-bf">consecutive</span> castles. Therefore the block from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span> will include castles <span class="tex-span"><i>i</i>, <i>i</i> + 1, ..., <i>j</i></span>. A block may consist of a single castle. </li><li> The partitioning is chosen in such a way that every castle is a part of <span class="tex-font-style-bf">exactly</span> one block. </li><li> Each block is sorted independently from other blocks, that is the sequence <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>h</i><sub class="lower-index"><i>j</i></sub></span> becomes sorted. </li><li> The partitioning should satisfy the condition that after each block is sorted, the sequence <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> becomes sorted too. This may always be achieved by saying that the whole sequence is a single block. </li></ul><p>Even Patrick understands that increasing the number of blocks in partitioning will ease the sorting process. Now friends ask you to count the maximum possible number of blocks in a partitioning that satisfies all the above requirements.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of castles Spongebob, Patrick and Squidward made from sand during the day.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The <span class="tex-span"><i>i</i></span>-th of these integers corresponds to the height of the <span class="tex-span"><i>i</i></span>-th castle.</p></div><div class="output-specification"><p>Print the maximum possible number of blocks in a valid partitioning.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of castles Spongebob, Patrick and Squidward made from sand during the day.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The <span class="tex-span"><i>i</i></span>-th of these integers corresponds to the height of the <span class="tex-span"><i>i</i></span>-th castle.</p>

## Output

<p>Print the maximum possible number of blocks in a valid partitioning.</p>





```input1
3
1 2 3

```




```input2
4
2 1 3 2

```




```output1
3

```




```output2
2

```



## Note

<p>In the first sample the partitioning looks like that: [1][2][3].</p><center> <img class="tex-graphics" height="227px" src="file://TxaZ8EDy.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>In the second sample the partitioning is: [2, 1][3, 2]</p><center> <img class="tex-graphics" height="227px" src="file://8kBLFLLX.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
