## Description

<div><p>Arkady decided to buy roses for his girlfriend.</p><p>A flower shop has white, orange and red roses, and the total amount of them is <span class="tex-span"><i>n</i></span>. Arkady thinks that red roses are not good together with white roses, so he won't buy a bouquet containing both red and white roses. Also, Arkady won't buy a bouquet where all roses have the same color. </p><p>Arkady wants to buy exactly <span class="tex-span"><i>k</i></span> roses. For each rose in the shop he knows its beauty and color: the beauty of the <span class="tex-span"><i>i</i></span>-th rose is <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and its color is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> ('<span class="tex-font-style-tt">W</span>' for a white rose, '<span class="tex-font-style-tt">O</span>' for an orange rose and '<span class="tex-font-style-tt">R</span>' for a red rose). </p><p>Compute the maximum possible total beauty of a bouquet of <span class="tex-span"><i>k</i></span> roses satisfying the constraints above or determine that it is not possible to make such a bouquet.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>) — the number of roses in the show and the number of roses Arkady wants to buy.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals the beauty of the <span class="tex-span"><i>i</i></span>-th rose.</p><p>The third line contains a string <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of uppercase English letters '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">O</span>' and '<span class="tex-font-style-tt">R</span>', where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> denotes the color of the <span class="tex-span"><i>i</i></span>-th rose: '<span class="tex-font-style-tt">W</span>' denotes white, '<span class="tex-font-style-tt">O</span>' &nbsp;— orange, '<span class="tex-font-style-tt">R</span>' — red.</p></div><div class="output-specification"><p>Print the maximum possible total beauty of a bouquet of <span class="tex-span"><i>k</i></span> roses that satisfies the constraints above. If it is not possible to make a single such bouquet, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>) — the number of roses in the show and the number of roses Arkady wants to buy.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals the beauty of the <span class="tex-span"><i>i</i></span>-th rose.</p><p>The third line contains a string <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of uppercase English letters '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">O</span>' and '<span class="tex-font-style-tt">R</span>', where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> denotes the color of the <span class="tex-span"><i>i</i></span>-th rose: '<span class="tex-font-style-tt">W</span>' denotes white, '<span class="tex-font-style-tt">O</span>' &nbsp;— orange, '<span class="tex-font-style-tt">R</span>' — red.</p>

## Output

<p>Print the maximum possible total beauty of a bouquet of <span class="tex-span"><i>k</i></span> roses that satisfies the constraints above. If it is not possible to make a single such bouquet, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 3
4 3 4 1 6
RROWW

```




```input2
5 2
10 20 14 20 11
RRRRR

```




```input3
11 5
5 6 3 2 3 4 7 5 4 5 6
RWOORWORROW

```




```output1
11

```




```output2
-1

```




```output3
28

```



## Note

<p>In the first example Arkady wants to buy <span class="tex-span">3</span> roses. He can, for example, buy both red roses (their indices are <span class="tex-span">1</span> and <span class="tex-span">2</span>, and their total beauty is <span class="tex-span">7</span>) and the only orange rose (its index is <span class="tex-span">3</span>, its beauty is <span class="tex-span">4</span>). This way the total beauty of the bouquet is <span class="tex-span">11</span>. </p><p>In the second example Arkady can not buy a bouquet because all roses have the same color.</p>
