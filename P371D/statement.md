## Description

<div><p>There is a system of <span class="tex-span"><i>n</i></span> vessels arranged one above the other as shown in the figure below. Assume that the vessels are numbered from 1 to <span class="tex-span"><i>n</i></span>, in the order from the highest to the lowest, the volume of the <span class="tex-span"><i>i</i></span>-th vessel is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> liters.</p><center> <img class="tex-graphics" src="file://MKU6CqJM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially, all the vessels are empty. In some vessels water is poured. All the water that overflows from the <span class="tex-span"><i>i</i></span>-th vessel goes to the <span class="tex-span">(<i>i</i> + 1)</span>-th one. The liquid that overflows from the <span class="tex-span"><i>n</i></span>-th vessel spills on the floor.</p><p>Your task is to simulate pouring water into the vessels. To do this, you will need to handle two types of queries:</p><ol> <li> Add <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> liters of water to the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th vessel; </li><li> Print the number of liters of water in the <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>-th vessel. </li></ol><p>When you reply to the second request you can assume that all the water poured up to this point, has already overflown between the vessels.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vessels (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the vessels' capacities (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The vessels' capacities do not necessarily increase from the top vessels to the bottom ones (see the second sample). The third line contains integer <span class="tex-span"><i>m</i></span> — the number of queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of one query. The query of the first type is represented as "<span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub></span>", the query of the second type is represented as "<span class="tex-span">2&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>For each query, print on a single line the number of liters of water in the corresponding vessel.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vessels (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the vessels' capacities (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The vessels' capacities do not necessarily increase from the top vessels to the bottom ones (see the second sample). The third line contains integer <span class="tex-span"><i>m</i></span> — the number of queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of one query. The query of the first type is represented as "<span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub></span>", the query of the second type is represented as "<span class="tex-span">2&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>For each query, print on a single line the number of liters of water in the corresponding vessel.</p>





```input1
2
5 10
6
1 1 4
2 1
1 2 5
1 1 4
2 1
2 2

```




```input2
3
5 10 8
6
1 1 12
2 2
1 1 6
1 3 2
2 2
2 3

```




```output1
4
5
8

```




```output2
7
10
5

```


