## Description

<div><p>A revolution took place on the Buka Island. New government replaced the old one. The new government includes <span class="tex-span"><i>n</i></span> parties and each of them is entitled to some part of the island according to their contribution to the revolution. However, they can't divide the island.</p><p>The island can be conventionally represented as two rectangles <span class="tex-span"><i>a</i> × <i>b</i></span> and <span class="tex-span"><i>c</i> × <i>d</i></span> unit squares in size correspondingly. The rectangles are located close to each other. At that, one of the sides with the length of <span class="tex-span"><i>a</i></span> and one of the sides with the length of <span class="tex-span"><i>c</i></span> lie on one line. You can see this in more details on the picture.</p><center> <img class="tex-graphics" src="file://vlnn2NxM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-span"><i>i</i></span>-th party is entitled to a part of the island equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> unit squares. Every such part should fully cover several squares of the island (it is not allowed to cover the squares partially) and be a connected figure. A "connected figure" presupposes that from any square of this party one can move to any other square of the same party moving through edge-adjacent squares also belonging to that party.</p><p>Your task is to divide the island between parties.</p></div><div class="input-specification"><p>The first line contains 5 space-separated integers — <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 50</span>, <span class="tex-span"><i>b</i> ≠ <i>d</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 26</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers. The <span class="tex-span"><i>i</i></span>-th of them is equal to number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i> × <i>b</i> + <i>c</i> × <i>d</i></span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://unrQCQdx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>If dividing the island between parties in the required manner is impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (also without the quotes) and, starting from the next line, print <span class="tex-span"><i>max</i>(<i>b</i>, <i>d</i>)</span> lines each containing <span class="tex-span"><i>a</i> + <i>c</i></span> characters. To mark what square should belong to what party, use lowercase Latin letters. For the party that is first in order in the input data, use "<span class="tex-font-style-tt">a</span>", for the second one use "<span class="tex-font-style-tt">b</span>" and so on. Use "<span class="tex-font-style-tt">.</span>" for the squares that belong to the sea. The first symbol of the second line of the output data should correspond to the square that belongs to the rectangle <span class="tex-span"><i>a</i> × <i>b</i></span>. The last symbol of the second line should correspond to the square that belongs to the rectangle <span class="tex-span"><i>c</i> × <i>d</i></span>.</p><p>If there are several solutions output any.</p></div>

## Input

<p>The first line contains 5 space-separated integers — <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 50</span>, <span class="tex-span"><i>b</i> ≠ <i>d</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 26</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers. The <span class="tex-span"><i>i</i></span>-th of them is equal to number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i> × <i>b</i> + <i>c</i> × <i>d</i></span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://unrQCQdx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>If dividing the island between parties in the required manner is impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (also without the quotes) and, starting from the next line, print <span class="tex-span"><i>max</i>(<i>b</i>, <i>d</i>)</span> lines each containing <span class="tex-span"><i>a</i> + <i>c</i></span> characters. To mark what square should belong to what party, use lowercase Latin letters. For the party that is first in order in the input data, use "<span class="tex-font-style-tt">a</span>", for the second one use "<span class="tex-font-style-tt">b</span>" and so on. Use "<span class="tex-font-style-tt">.</span>" for the squares that belong to the sea. The first symbol of the second line of the output data should correspond to the square that belongs to the rectangle <span class="tex-span"><i>a</i> × <i>b</i></span>. The last symbol of the second line should correspond to the square that belongs to the rectangle <span class="tex-span"><i>c</i> × <i>d</i></span>.</p><p>If there are several solutions output any.</p>





```input1
3 4 2 2 3
5 8 3

```




```input2
3 2 1 4 4
1 2 3 4

```




```output1
YES
aaabb
aabbb
cbb..
ccb..

```




```output2
YES
abbd
cccd
...d
...d

```


