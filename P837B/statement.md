## Description

<div><p>The flag of Berland is such rectangular field <span class="tex-span"><i>n</i> × <i>m</i></span> that satisfies following conditions:</p><ul> <li> Flag consists of three colors which correspond to letters <span class="tex-font-style-tt">'R'</span>, <span class="tex-font-style-tt">'G'</span> and <span class="tex-font-style-tt">'B'</span>. </li><li> Flag consists of three equal in width and height stripes, parralel to each other and to sides of the flag. Each stripe has <span class="tex-font-style-bf">exactly one color</span>. </li><li> Each color should be used in <span class="tex-font-style-bf">exactly one stripe</span>. </li></ul><p>You are given a field <span class="tex-span"><i>n</i> × <i>m</i></span>, consisting of characters <span class="tex-font-style-tt">'R'</span>, <span class="tex-font-style-tt">'G'</span> and <span class="tex-font-style-tt">'B'</span>. Output "<span class="tex-font-style-tt">YES</span>" (without quotes) if this field corresponds to correct flag of Berland. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the sizes of the field.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines consisting of <span class="tex-span"><i>m</i></span> characters <span class="tex-font-style-tt">'R'</span>, <span class="tex-font-style-tt">'G'</span> and <span class="tex-font-style-tt">'B'</span> — the description of the field.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the given field corresponds to correct flag of Berland . Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the sizes of the field.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines consisting of <span class="tex-span"><i>m</i></span> characters <span class="tex-font-style-tt">'R'</span>, <span class="tex-font-style-tt">'G'</span> and <span class="tex-font-style-tt">'B'</span> — the description of the field.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the given field corresponds to correct flag of Berland . Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
6 5
RRRRR
RRRRR
BBBBB
BBBBB
GGGGG
GGGGG

```




```input2
4 3
BRG
BRG
BRG
BRG

```




```input3
6 7
RRRGGGG
RRRGGGG
RRRGGGG
RRRBBBB
RRRBBBB
RRRBBBB

```




```input4
4 4
RRRR
RRRR
BBBB
GGGG

```




```output1
YES

```




```output2
YES

```




```output3
NO

```




```output4
NO

```



## Note

<p>The field in the third example doesn't have three parralel stripes.</p><p>Rows of the field in the fourth example are parralel to each other and to borders. But they have different heights — <span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">1</span> and <span class="tex-font-style-tt">1</span>.</p>
