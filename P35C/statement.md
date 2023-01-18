## Description

<div><p>After a terrifying forest fire in Berland a forest rebirth program was carried out. Due to it <span class="tex-span"><i>N</i></span> rows with <span class="tex-span"><i>M</i></span> trees each were planted and the rows were so neat that one could map it on a system of coordinates so that the <span class="tex-span"><i>j</i></span>-th tree in the <span class="tex-span"><i>i</i></span>-th row would have the coordinates of <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. However a terrible thing happened and the young forest caught fire. Now we must find the coordinates of the tree that will catch fire last to plan evacuation.</p><p>The burning began in <span class="tex-span"><i>K</i></span> points simultaneously, which means that initially <span class="tex-span"><i>K</i></span> trees started to burn. Every minute the fire gets from the burning trees to the ones that aren’t burning and that the distance from them to the nearest burning tree equals to 1.</p><p>Find the tree that will be the last to start burning. If there are several such trees, output any.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>N</i>, <i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 2000</span>) — the size of the forest. The trees were planted in all points of the (<span class="tex-span"><i>x</i>, <i>y</i></span>) (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>N</i>, 1 ≤ <i>y</i> ≤ <i>M</i></span>) type, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are integers.</p><p>The second line contains an integer <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 10</span>) — amount of trees, burning in the beginning. </p><p>The third line contains <span class="tex-span"><i>K</i></span> pairs of integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>M</i></span>) — coordinates of the points from which the fire started. It is guaranteed that no two points coincide.</p></div><div class="output-specification"><p>Output a line with two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — coordinates of the tree that will be the last one to start burning. If there are several such trees, output any.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>N</i>, <i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 2000</span>) — the size of the forest. The trees were planted in all points of the (<span class="tex-span"><i>x</i>, <i>y</i></span>) (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>N</i>, 1 ≤ <i>y</i> ≤ <i>M</i></span>) type, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are integers.</p><p>The second line contains an integer <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 10</span>) — amount of trees, burning in the beginning. </p><p>The third line contains <span class="tex-span"><i>K</i></span> pairs of integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>M</i></span>) — coordinates of the points from which the fire started. It is guaranteed that no two points coincide.</p>

## Output

<p>Output a line with two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — coordinates of the tree that will be the last one to start burning. If there are several such trees, output any.</p>





```input1
3 3
1
2 2

```




```input2
3 3
1
1 1

```




```input3
3 3
2
1 1 3 3

```




```output1
1 1

```




```output2
3 3

```




```output3
2 2
```


