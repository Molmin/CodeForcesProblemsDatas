## Description

<div><p>Like all children, Alesha loves New Year celebration. During the celebration he and his whole family dress up the fir-tree. Like all children, Alesha likes to play with garlands&nbsp;— chains consisting of a lightbulbs.</p><p>Alesha uses a grid field sized <span class="tex-span"><i>n</i> × <i>m</i></span> for playing. The rows of the field are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the top to the bottom and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from the left to the right.</p><p>Alesha has <span class="tex-span"><i>k</i></span> garlands which he places at the field. He does so in the way such that each lightbulb of each garland lies in the center of some cell in the field, and each cell contains <span class="tex-font-style-bf">at most one lightbulb</span>. Of course lightbulbs, which are neighbours in some garland, appears in cells neighbouring by a side.</p><center><p><img class="tex-graphics" src="file://U2DQwiCY.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The example of garland placing.</p></center><p>Each garland is turned off or turned on at any moment. If some garland is turned on then each of its lightbulbs is turned on, the same applies for garland turned off. Each lightbulb in the whole garland set is unique, and thus, being turned on, brings Alesha some pleasure, described by an integer value. Turned off lightbulbs don't bring Alesha any pleasure.</p><p>Alesha can turn garlands on and off and wants to know the sum of pleasure value which the lightbulbs, placed in the centers of the cells in some rectangular part of the field, bring him. Initially <span class="tex-font-style-bf">all the garlands are turned on</span>.</p><p>Alesha is still very little and can't add big numbers. He extremely asks you to help him.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>)&nbsp;— the number of field rows, the number of field columns and the number of garlands placed at the field respectively.</p><p>Next lines contains garlands set description in the following format:</p><p>The first line of a single garland description contains a single integer <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ 2000</span>)&nbsp;— the number of lightbulbs in the garland.</p><p>Each of the next <span class="tex-span"><i>len</i></span> lines contains three integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the cell containing a lightbullb and pleasure value Alesha gets from it if it is turned on. The lightbulbs are given in the order they are forming a chain in the garland. It is guaranteed that neighbouring lightbulbs are placed in the cells neighbouring by a side.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of events in Alesha's game. The next <span class="tex-span"><i>q</i></span> lines describes events in chronological order. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th event in the one of the following formats:</p><ul> <li> <span class="tex-font-style-tt">SWITCH</span> <span class="tex-span"><i>i</i></span>&nbsp;— Alesha turns off <span class="tex-span"><i>i</i></span>-th garland if it is turned on, or turns it on if it is turned off. It is guaranteed that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>. </li><li> <span class="tex-font-style-tt">ASK</span> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>&nbsp;— Alesha wants to know the sum of pleasure values the lightbulbs, placed in a rectangular part of the field. Top-left cell of a part has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and right-bottom cell has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>. It is guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>. There is <span class="tex-font-style-bf">no more than <span class="tex-span">2000</span></span> events of this type in the input. </li></ul><p>All the numbers in the input are integers.</p><p>Please note that the input is quite large, so be careful while using some input ways. In particular, it's not recommended to use <span class="tex-font-style-tt">cin</span> in codes on <span class="tex-font-style-tt">C++</span> and class <span class="tex-font-style-tt">Scanner</span> in codes on <span class="tex-font-style-tt">Java</span>.</p></div><div class="output-specification"><p>For each <span class="tex-font-style-tt">ASK</span> operation print the sum Alesha wants to know in a separate line. Print the answers in chronological order.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>)&nbsp;— the number of field rows, the number of field columns and the number of garlands placed at the field respectively.</p><p>Next lines contains garlands set description in the following format:</p><p>The first line of a single garland description contains a single integer <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ 2000</span>)&nbsp;— the number of lightbulbs in the garland.</p><p>Each of the next <span class="tex-span"><i>len</i></span> lines contains three integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the cell containing a lightbullb and pleasure value Alesha gets from it if it is turned on. The lightbulbs are given in the order they are forming a chain in the garland. It is guaranteed that neighbouring lightbulbs are placed in the cells neighbouring by a side.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of events in Alesha's game. The next <span class="tex-span"><i>q</i></span> lines describes events in chronological order. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th event in the one of the following formats:</p><ul> <li> <span class="tex-font-style-tt">SWITCH</span> <span class="tex-span"><i>i</i></span>&nbsp;— Alesha turns off <span class="tex-span"><i>i</i></span>-th garland if it is turned on, or turns it on if it is turned off. It is guaranteed that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>. </li><li> <span class="tex-font-style-tt">ASK</span> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>&nbsp;— Alesha wants to know the sum of pleasure values the lightbulbs, placed in a rectangular part of the field. Top-left cell of a part has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and right-bottom cell has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>. It is guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>. There is <span class="tex-font-style-bf">no more than <span class="tex-span">2000</span></span> events of this type in the input. </li></ul><p>All the numbers in the input are integers.</p><p>Please note that the input is quite large, so be careful while using some input ways. In particular, it's not recommended to use <span class="tex-font-style-tt">cin</span> in codes on <span class="tex-font-style-tt">C++</span> and class <span class="tex-font-style-tt">Scanner</span> in codes on <span class="tex-font-style-tt">Java</span>.</p>

## Output

<p>For each <span class="tex-font-style-tt">ASK</span> operation print the sum Alesha wants to know in a separate line. Print the answers in chronological order.</p>





```input1
4 4 3
5
1 1 2
1 2 3
2 2 1
2 1 4
3 1 7
4
1 3 1
2 3 3
2 4 3
1 4 1
7
4 1 1
4 2 9
3 2 8
3 3 3
4 3 4
4 4 1
3 4 1
2
ASK 2 2 3 3
ASK 1 1 4 4

```




```input2
4 4 1
8
4 1 1
3 1 2
2 1 1
1 1 7
1 2 5
2 2 4
2 3 1
1 3 1
3
ASK 1 1 3 2
SWITCH 1
ASK 1 1 3 2

```




```output1
15
52

```




```output2
19
0

```



## Note

<center><p><img class="tex-graphics" src="file://ChKp4od1.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This image illustrates the first sample case.</p></center>
