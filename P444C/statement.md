## Description

<div><p><span class="tex-font-style-it">DZY loves colors, and he enjoys painting.</span></p><p>On a colorful day, DZY gets a colorful ribbon, which consists of <span class="tex-span"><i>n</i></span> units (they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right). The color of the <span class="tex-span"><i>i</i></span>-th unit of the ribbon is <span class="tex-span"><i>i</i></span> at first. It is colorful enough, but we still consider that the colorfulness of each unit is <span class="tex-span">0</span> at first.</p><p>DZY loves painting, we know. He takes up a paintbrush with color <span class="tex-span"><i>x</i></span> and uses it to draw a line on the ribbon. In such a case some contiguous units are painted. Imagine that the color of unit <span class="tex-span"><i>i</i></span> currently is <span class="tex-span"><i>y</i></span>. When it is painted by this paintbrush, the color of the unit becomes <span class="tex-span"><i>x</i></span>, and the colorfulness of the unit increases by <span class="tex-span">|<i>x</i> - <i>y</i>|</span>.</p><p>DZY wants to perform <span class="tex-span"><i>m</i></span> operations, each operation can be one of the following:</p><ol> <li> Paint all the units with numbers between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (both inclusive) with color <span class="tex-span"><i>x</i></span>. </li><li> Ask the sum of colorfulness of the units between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (both inclusive). </li></ol><p>Can you help DZY?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines begins with a integer <span class="tex-span"><i>type</i>&nbsp;(1 ≤ <i>type</i> ≤ 2)</span>, which represents the type of this operation.</p><p>If <span class="tex-span"><i>type</i> = 1</span>, there will be <span class="tex-span">3</span> more integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">8</sup>)</span> in this line, describing an operation <span class="tex-span">1</span>.</p><p>If <span class="tex-span"><i>type</i> = 2</span>, there will be <span class="tex-span">2</span> more integers <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> in this line, describing an operation <span class="tex-span">2</span>.</p></div><div class="output-specification"><p>For each operation <span class="tex-span">2</span>, print a line containing the answer — sum of colorfulness.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines begins with a integer <span class="tex-span"><i>type</i>&nbsp;(1 ≤ <i>type</i> ≤ 2)</span>, which represents the type of this operation.</p><p>If <span class="tex-span"><i>type</i> = 1</span>, there will be <span class="tex-span">3</span> more integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">8</sup>)</span> in this line, describing an operation <span class="tex-span">1</span>.</p><p>If <span class="tex-span"><i>type</i> = 2</span>, there will be <span class="tex-span">2</span> more integers <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> in this line, describing an operation <span class="tex-span">2</span>.</p>

## Output

<p>For each operation <span class="tex-span">2</span>, print a line containing the answer — sum of colorfulness.</p>





```input1
3 3
1 1 2 4
1 2 3 5
2 1 3

```




```input2
3 4
1 1 3 4
2 1 1
2 2 2
2 3 3

```




```input3
10 6
1 1 5 3
1 2 7 9
1 10 10 11
1 3 8 12
1 1 10 3
2 1 10

```




```output1
8

```




```output2
3
2
1

```




```output3
129

```



## Note

<p>In the first sample, the color of each unit is initially <span class="tex-span">[1, 2, 3]</span>, and the colorfulness is <span class="tex-span">[0, 0, 0]</span>.</p><p>After the first operation, colors become <span class="tex-span">[4, 4, 3]</span>, colorfulness become <span class="tex-span">[3, 2, 0]</span>.</p><p>After the second operation, colors become <span class="tex-span">[4, 5, 5]</span>, colorfulness become <span class="tex-span">[3, 3, 2]</span>.</p><p>So the answer to the only operation of type <span class="tex-span">2</span> is <span class="tex-span">8</span>.</p>
