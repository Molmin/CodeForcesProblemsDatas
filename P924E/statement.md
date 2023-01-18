## Description

<div><p>Olya wants to buy a custom wardrobe. It should have <span class="tex-span"><i>n</i></span> boxes with heights <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, stacked one on another in some order. In other words, we can represent each box as a vertical segment of length <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and all these segments should form a single segment from <span class="tex-span">0</span> to <img align="middle" class="tex-formula" src="file://vV7LGydf.png" style="max-width: 100.0%;max-height: 100.0%;"> without any overlaps.</p><p>Some of the boxes are important (in this case <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 1</span>), others are not (then <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span>). Olya defines the <span class="tex-font-style-it">convenience</span> of the wardrobe as the number of important boxes such that their bottom edge is located between the heights <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive.</p><p>You are given information about heights of the boxes and their importance. Compute the maximum possible convenience of the wardrobe if you can reorder the boxes arbitrarily.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ 10 000</span>)&nbsp;— the number of boxes, the lowest and the highest heights for a bottom edge of an important box to be counted in convenience.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the heights of the boxes. It is guaranteed that the sum of height of all boxes (i.&nbsp;e. the height of the wardrobe) does not exceed <span class="tex-span">10 000</span>: Olya is not very tall and will not be able to reach any higher.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th box is important, and <span class="tex-span">0</span> otherwise.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible convenience of the wardrobe.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ 10 000</span>)&nbsp;— the number of boxes, the lowest and the highest heights for a bottom edge of an important box to be counted in convenience.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the heights of the boxes. It is guaranteed that the sum of height of all boxes (i.&nbsp;e. the height of the wardrobe) does not exceed <span class="tex-span">10 000</span>: Olya is not very tall and will not be able to reach any higher.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th box is important, and <span class="tex-span">0</span> otherwise.</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible convenience of the wardrobe.</p>





```input1
5 3 6
3 2 5 1 2
1 1 0 1 0

```




```input2
2 2 5
3 6
1 1

```




```output1
2

```




```output2
1

```



## Note

<p>In the first example you can, for example, first put an unimportant box of height <span class="tex-span">2</span>, then put an important boxes of sizes <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">2</span>, in this order, and then the remaining unimportant boxes. The convenience is equal to <span class="tex-span">2</span>, because the bottom edges of important boxes of sizes <span class="tex-span">3</span> and <span class="tex-span">2</span> fall into the range <span class="tex-span">[3, 6]</span>.</p><p>In the second example you have to put the short box under the tall box.</p>
