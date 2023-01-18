## Description

<div><p>Dasha is fond of challenging puzzles: Rubik's Cube <span class="tex-span">3 × 3 × 3</span>, <span class="tex-span">4 × 4 × 4</span>, <span class="tex-span">5 × 5 × 5</span> and so on. This time she has a cyclic table of size <span class="tex-span"><i>n</i> × <i>m</i></span>, and each cell of the table contains a lowercase English letter. Each cell has coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">0 ≤ <i>i</i> &lt; <i>n</i></span>, <span class="tex-span">0 ≤ <i>j</i> &lt; <i>m</i></span>). The table is cyclic means that to the right of cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> there is the cell <img align="middle" class="tex-formula" src="file://Hw4J8Q3p.png" style="max-width: 100.0%;max-height: 100.0%;">, and to the down there is the cell <img align="middle" class="tex-formula" src="file://0vgnVwbM.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Dasha has a pattern as well. A pattern is a non-cyclic table of size <span class="tex-span"><i>r</i> × <i>c</i></span>. Each cell is either a lowercase English letter or a question mark. Each cell has coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">0 ≤ <i>i</i> &lt; <i>r</i></span>, <span class="tex-span">0 ≤ <i>j</i> &lt; <i>c</i></span>).</p><p>The goal of the puzzle is to find all the appearance positions of the pattern in the cyclic table.</p><p>We say that the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> of cyclic table is an appearance position, if for every pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span">0 ≤ <i>x</i> &lt; <i>r</i></span> and <span class="tex-span">0 ≤ <i>y</i> &lt; <i>c</i></span> one of the following conditions holds: </p><ul> <li> There is a question mark in the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the pattern, or </li><li> The cell <img align="middle" class="tex-formula" src="file://sIYQTOsl.png" style="max-width: 100.0%;max-height: 100.0%;"> of the cyclic table equals to the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the pattern. </li></ul><p>Dasha solved this puzzle in no time, as well as all the others she ever tried. Can you solve it?.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 400</span>)&nbsp;— the cyclic table sizes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> lowercase English characters&nbsp;— the description of the cyclic table.</p><p>The next line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>c</i> ≤ 400</span>)&nbsp;— the sizes of the pattern.</p><p>Each of the next <span class="tex-span"><i>r</i></span> lines contains a string of <span class="tex-span"><i>c</i></span> lowercase English letter and/or characters '<span class="tex-font-style-tt">?</span>'&nbsp;— the description of the pattern.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. Each of the <span class="tex-span"><i>n</i></span> lines should contain <span class="tex-span"><i>m</i></span> characters. Each of the characters should equal '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p><p>The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">0</span>-indexed) line should be equal to '<span class="tex-font-style-tt">1</span>', in case the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is an appearance position, otherwise it should be equal to '<span class="tex-font-style-tt">0</span>'.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 400</span>)&nbsp;— the cyclic table sizes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> lowercase English characters&nbsp;— the description of the cyclic table.</p><p>The next line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>c</i> ≤ 400</span>)&nbsp;— the sizes of the pattern.</p><p>Each of the next <span class="tex-span"><i>r</i></span> lines contains a string of <span class="tex-span"><i>c</i></span> lowercase English letter and/or characters '<span class="tex-font-style-tt">?</span>'&nbsp;— the description of the pattern.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. Each of the <span class="tex-span"><i>n</i></span> lines should contain <span class="tex-span"><i>m</i></span> characters. Each of the characters should equal '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'.</p><p>The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">0</span>-indexed) line should be equal to '<span class="tex-font-style-tt">1</span>', in case the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is an appearance position, otherwise it should be equal to '<span class="tex-font-style-tt">0</span>'.</p>





```input1
5 7
qcezchs
hhedywq
wikywqy
qckrqzt
bqexcxz
3 2
??
yw
?q

```




```input2
10 10
fwtoayylhw
yyaryyjawr
ywrdzwhscy
hnsyyxiphn
bnjwzyyjvo
kkjgseenwn
gvmiflpcsy
lxvkwrobwu
wyybbcocyy
yysijsvqry
2 2
??
yy

```




```input3
8 6
ibrgxl
xqdcsg
okbcgi
tvpetc
xgxxig
igghzo
lmlaza
gpswzv
1 4
gx??

```




```output1
0000100
0001001
0000000
0000000
0000000

```




```output2
1000100000
0000000001
0001000000
0000010000
0000000000
0000000000
0000000000
0100000010
1000000001
0000010000

```




```output3
000100
000001
000000
000000
010001
000000
000000
000000

```


