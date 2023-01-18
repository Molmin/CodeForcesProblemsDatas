## Description

<div><p>User ainta decided to paint a wall. The wall consists of <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> tiles, that are arranged in an <span class="tex-span"><i>n</i> × <i>n</i></span> table. Some tiles are painted, and the others are not. As he wants to paint it beautifully, he will follow the rules below.</p><ol> <li> Firstly user ainta looks at the wall. If there is at least one painted cell on each row and at least one painted cell on each column, he stops coloring. Otherwise, he goes to step 2. </li><li> User ainta choose any tile on the wall with uniform probability. </li><li> If the tile he has chosen is not painted, he paints the tile. Otherwise, he ignores it. </li><li> Then he takes a rest for one minute even if he doesn't paint the tile. And then ainta goes to step 1. </li></ol> &nbsp;<p>However ainta is worried if it would take too much time to finish this work. So he wants to calculate the expected time needed to paint the wall by the method above. Help him find the expected time. You can assume that choosing and painting any tile consumes no time at all. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">3</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i><sup class="upper-index">2</sup>, 2·10<sup class="upper-index">4</sup>)</span>) — the size of the wall and the number of painted cells.</p><p>Next <span class="tex-span"><i>m</i></span> lines goes, each contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the position of the painted cell. It is guaranteed that the positions are all distinct. Consider the rows of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Consider the columns of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>In a single line print the expected time to paint the wall in minutes. Your answer will be considered correct if it has at most <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> absolute or relative error.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">3</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i><sup class="upper-index">2</sup>, 2·10<sup class="upper-index">4</sup>)</span>) — the size of the wall and the number of painted cells.</p><p>Next <span class="tex-span"><i>m</i></span> lines goes, each contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the position of the painted cell. It is guaranteed that the positions are all distinct. Consider the rows of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Consider the columns of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>In a single line print the expected time to paint the wall in minutes. Your answer will be considered correct if it has at most <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> absolute or relative error.</p>





```input1
5 2
2 3
4 1

```




```input2
2 2
1 1
1 2

```




```input3
1 1
1 1

```




```output1
11.7669491886

```




```output2
2.0000000000

```




```output3
0.0000000000

```


