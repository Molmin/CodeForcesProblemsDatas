## Description

<div><p>ZS the Coder and Chris the Baboon has arrived at Udayland! They walked in the park where <span class="tex-span"><i>n</i></span> trees grow. They decided to be naughty and color the trees in the park. The trees are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p><p>Initially, tree <span class="tex-span"><i>i</i></span> has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. ZS the Coder and Chris the Baboon recognizes only <span class="tex-span"><i>m</i></span> different colors, so <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = 0</span> means that tree <span class="tex-span"><i>i</i></span> is <span class="tex-font-style-it">uncolored</span>.</p><p>ZS the Coder and Chris the Baboon decides to color only the uncolored trees, i.e. the trees with <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = 0</span>. They can color each of them them in any of the <span class="tex-span"><i>m</i></span> colors from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Coloring the <span class="tex-span"><i>i</i></span>-th tree with color <span class="tex-span"><i>j</i></span> requires exactly <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> litres of paint.</p><p>The two friends define the <span class="tex-font-style-it">beauty</span> of a coloring of the trees as the <span class="tex-font-style-bf">minimum</span> number of contiguous groups (each group contains some subsegment of trees) you can split all the <span class="tex-span"><i>n</i></span> trees into so that each group contains trees of the same color. For example, if the colors of the trees from left to right are <span class="tex-span">2, 1, 1, 1, 3, 2, 2, 3, 1, 3</span>, the beauty of the coloring is <span class="tex-span">7</span>, since we can partition the trees into <span class="tex-span">7</span> contiguous groups of the same color : <span class="tex-span">{2}, {1, 1, 1}, {3}, {2, 2}, {3}, {1}, {3}</span>. </p><p>ZS the Coder and Chris the Baboon wants to color all uncolored trees so that the beauty of the coloring is <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span>. They need your help to determine the minimum amount of paint (in litres) needed to finish the job.</p><p>Please note that the friends can't color the trees that are already colored.</p></div><div class="input-specification"><p>The first line contains three integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of trees, number of colors and beauty of the resulting coloring respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), the initial colors of the trees. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span">0</span> if the tree number <span class="tex-span"><i>i</i></span> is uncolored, otherwise the <span class="tex-span"><i>i</i></span>-th tree has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. Each of them contains <span class="tex-span"><i>m</i></span> integers. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th of them line denotes <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the amount of litres the friends need to color <span class="tex-span"><i>i</i></span>-th tree with color <span class="tex-span"><i>j</i></span>. <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>'s are specified even for the initially colored trees, but such trees still can't be colored.</p></div><div class="output-specification"><p>Print a single integer, the minimum amount of paint needed to color the trees. If there are no valid tree colorings of beauty <span class="tex-span"><i>k</i></span>, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains three integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of trees, number of colors and beauty of the resulting coloring respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), the initial colors of the trees. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span">0</span> if the tree number <span class="tex-span"><i>i</i></span> is uncolored, otherwise the <span class="tex-span"><i>i</i></span>-th tree has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. Each of them contains <span class="tex-span"><i>m</i></span> integers. The <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th of them line denotes <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the amount of litres the friends need to color <span class="tex-span"><i>i</i></span>-th tree with color <span class="tex-span"><i>j</i></span>. <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>'s are specified even for the initially colored trees, but such trees still can't be colored.</p>

## Output

<p>Print a single integer, the minimum amount of paint needed to color the trees. If there are no valid tree colorings of beauty <span class="tex-span"><i>k</i></span>, print <span class="tex-span"> - 1</span>.</p>





```input1
3 2 2
0 0 0
1 2
3 4
5 6

```




```input2
3 2 2
2 1 2
1 3
2 4
3 5

```




```input3
3 2 2
2 0 0
1 3
2 4
3 5

```




```input4
3 2 3
2 1 2
1 3
2 4
3 5

```




```output1
10
```




```output2
-1
```




```output3
5
```




```output4
0
```



## Note

<p>In the first sample case, coloring the trees with colors <span class="tex-span">2, 1, 1</span> minimizes the amount of paint used, which equals to <span class="tex-span">2 + 3 + 5 = 10</span>. Note that <span class="tex-span">1, 1, 1</span> would not be valid because the beauty of such coloring equals to <span class="tex-span">1</span> (<span class="tex-span">{1, 1, 1}</span> is a way to group the trees into a single group of the same color).</p><p>In the second sample case, all the trees are colored, but the beauty of the coloring is <span class="tex-span">3</span>, so there is no valid coloring, and the answer is <span class="tex-span"> - 1</span>.</p><p>In the last sample case, all the trees are colored and the beauty of the coloring matches <span class="tex-span"><i>k</i></span>, so no paint is used and the answer is <span class="tex-span">0</span>. </p>
