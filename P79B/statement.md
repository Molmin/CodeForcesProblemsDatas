## Description

<div><p>Fox Ciel saw a large field while she was on a bus. The field was a <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle divided into <span class="tex-span">1 × 1</span> cells. Some cells were wasteland, and other each cell contained crop plants: either carrots or kiwis or grapes. </p><p>After seeing the field carefully, Ciel found that the crop plants of each cell were planted in following procedure:</p><ul> <li> Assume that the rows are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and the columns are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right, and a cell in row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span> is represented as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. </li><li> First, each field is either cultivated or waste. Crop plants will be planted in the cultivated cells in the order of <span class="tex-span">(1, 1) → ... → (1, <i>m</i>) → (2, 1) → ... → (2, <i>m</i>) → ... → (<i>n</i>, 1) → ... → (<i>n</i>, <i>m</i>)</span>. Waste cells will be ignored. </li><li> Crop plants (either carrots or kiwis or grapes) will be planted in each cell one after another cyclically. Carrots will be planted in the first cell, then kiwis in the second one, grapes in the third one, carrots in the forth one, kiwis in the fifth one, and so on. </li></ul><p>The following figure will show you the example of this procedure. Here, a white square represents a cultivated cell, and a black square represents a waste cell.</p><center> <img class="tex-graphics" src="file://P1Q9LiMQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now she is wondering how to determine the crop plants in some certain cells. </p></div><div class="input-specification"><p>In the first line there are four positive integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">4</sup>, 1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">3</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">3</sup></span>), each of which represents the height of the field, the width of the field, the number of waste cells and the number of queries that ask the kind of crop plants in a certain cell.</p><p>Following each <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i>, 1 ≤ <i>b</i> ≤ <i>m</i></span>), which denotes a cell <span class="tex-span">(<i>a</i>, <i>b</i>)</span> is waste. It is guaranteed that the same cell will not appear twice in this section.</p><p>Following each <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>j</i> ≤ <i>m</i></span>), which is a query that asks you the kind of crop plants of a cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p></div><div class="output-specification"><p>For each query, if the cell is waste, print <span class="tex-font-style-tt">Waste</span>. Otherwise, print the name of crop plants in the cell: either <span class="tex-font-style-tt">Carrots</span> or <span class="tex-font-style-tt">Kiwis</span> or <span class="tex-font-style-tt">Grapes</span>.</p></div>

## Input

<p>In the first line there are four positive integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">4</sup>, 1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">3</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">3</sup></span>), each of which represents the height of the field, the width of the field, the number of waste cells and the number of queries that ask the kind of crop plants in a certain cell.</p><p>Following each <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i>, 1 ≤ <i>b</i> ≤ <i>m</i></span>), which denotes a cell <span class="tex-span">(<i>a</i>, <i>b</i>)</span> is waste. It is guaranteed that the same cell will not appear twice in this section.</p><p>Following each <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>j</i> ≤ <i>m</i></span>), which is a query that asks you the kind of crop plants of a cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p>

## Output

<p>For each query, if the cell is waste, print <span class="tex-font-style-tt">Waste</span>. Otherwise, print the name of crop plants in the cell: either <span class="tex-font-style-tt">Carrots</span> or <span class="tex-font-style-tt">Kiwis</span> or <span class="tex-font-style-tt">Grapes</span>.</p>





```input1
4 5 5 6
4 3
1 3
3 3
2 5
3 2
1 3
1 4
2 3
2 4
1 1
1 1

```




```output1
Waste
Grapes
Carrots
Kiwis
Carrots
Carrots

```



## Note

<p>The sample corresponds to the figure in the statement.</p>
