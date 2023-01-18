## Description

<div><p><span class="tex-font-style-it">I won't feel lonely, nor will I be sorrowful... not before everything is buried.</span></p><p>A string of <span class="tex-span"><i>n</i></span> beads is left as the message of leaving. The beads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right, each having a shape numbered by integers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive. Some beads may have the same shapes.</p><p>The <span class="tex-font-style-underline">memory</span> of a shape <span class="tex-span"><i>x</i></span> in a certain subsegment of beads, is defined to be the difference between the last position and the first position that shape <span class="tex-span"><i>x</i></span> appears in the segment. The <span class="tex-font-style-underline">memory</span> of a subsegment is the sum of <span class="tex-font-style-underline">memories</span> over all shapes that occur in it.</p><p>From time to time, shapes of beads change as well as the <span class="tex-font-style-underline">memories</span>. Sometimes, the past secreted in subsegments are being recalled, and you are to find the <span class="tex-font-style-underline">memory</span> for each of them.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>) — the number of beads in the string, and the total number of changes and queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the initial shapes of beads <span class="tex-span">1, 2, ..., <i>n</i></span>, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines each describes either a change in the beads or a query of subsegment. A line has one of the following formats: </p><ul> <li> <span class="tex-font-style-tt">1 p x</span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), meaning that the shape of the <span class="tex-span"><i>p</i></span>-th bead is changed into <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), denoting a query of <span class="tex-font-style-underline">memory</span> of the subsegment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive. </li></ul></div><div class="output-specification"><p>For each query, print one line with an integer — the <span class="tex-font-style-underline">memory</span> of the recalled subsegment.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>) — the number of beads in the string, and the total number of changes and queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the initial shapes of beads <span class="tex-span">1, 2, ..., <i>n</i></span>, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines each describes either a change in the beads or a query of subsegment. A line has one of the following formats: </p><ul> <li> <span class="tex-font-style-tt">1 p x</span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), meaning that the shape of the <span class="tex-span"><i>p</i></span>-th bead is changed into <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), denoting a query of <span class="tex-font-style-underline">memory</span> of the subsegment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive. </li></ul>

## Output

<p>For each query, print one line with an integer — the <span class="tex-font-style-underline">memory</span> of the recalled subsegment.</p>





```input1
7 6
1 2 3 1 3 2 1
2 3 7
2 1 3
1 7 2
1 3 2
2 1 6
2 5 7

```




```input2
7 5
1 3 2 1 4 2 3
1 1 4
2 2 3
1 1 7
2 4 5
1 1 7

```




```output1
5
0
7
1

```




```output2
0
0

```



## Note

<p>The initial string of beads has shapes <span class="tex-span">(1, 2, 3, 1, 3, 2, 1)</span>.</p><p>Consider the changes and queries in their order: </p><ol> <li> <span class="tex-font-style-tt">2 3 7</span>: the <span class="tex-font-style-underline">memory</span> of the subsegment <span class="tex-span">[3, 7]</span> is <span class="tex-span">(7 - 4) + (6 - 6) + (5 - 3) = 5</span>; </li><li> <span class="tex-font-style-tt">2 1 3</span>: the <span class="tex-font-style-underline">memory</span> of the subsegment <span class="tex-span">[1, 3]</span> is <span class="tex-span">(1 - 1) + (2 - 2) + (3 - 3) = 0</span>; </li><li> <span class="tex-font-style-tt">1 7 2</span>: the shape of the <span class="tex-span">7</span>-th bead changes into <span class="tex-span">2</span>. Beads now have shapes <span class="tex-span">(1, 2, 3, 1, 3, 2, 2)</span> respectively; </li><li> <span class="tex-font-style-tt">1 3 2</span>: the shape of the <span class="tex-span">3</span>-rd bead changes into <span class="tex-span">2</span>. Beads now have shapes <span class="tex-span">(1, 2, 2, 1, 3, 2, 2)</span> respectively; </li><li> <span class="tex-font-style-tt">2 1 6</span>: the <span class="tex-font-style-underline">memory</span> of the subsegment <span class="tex-span">[1, 6]</span> is <span class="tex-span">(4 - 1) + (6 - 2) + (5 - 5) = 7</span>; </li><li> <span class="tex-font-style-tt">2 5 7</span>: the <span class="tex-font-style-underline">memory</span> of the subsegment <span class="tex-span">[5, 7]</span> is <span class="tex-span">(7 - 6) + (5 - 5) = 1</span>. </li></ol>
