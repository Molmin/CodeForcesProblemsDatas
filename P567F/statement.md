## Description

<div><p>King of Berland Berl IV has recently died. Hail Berl V! As a sign of the highest achievements of the deceased king the new king decided to build a mausoleum with Berl IV's body on the main square of the capital.</p><p>The mausoleum will be constructed from <span class="tex-span">2<i>n</i></span> blocks, each of them has the shape of a cuboid. Each block has the bottom base of a <span class="tex-span">1 × 1</span> meter square. Among the blocks, exactly two of them have the height of one meter, exactly two have the height of two meters, ..., exactly two have the height of <span class="tex-span"><i>n</i></span> meters.</p><p>The blocks are arranged in a row without spacing one after the other. Of course, not every arrangement of blocks has the form of a mausoleum. In order to make the given arrangement in the form of the mausoleum, it is necessary that when you pass along the mausoleum, from one end to the other, the heights of the blocks first were <span class="tex-font-style-it">non-decreasing</span> (i.e., increasing or remained the same), and then — <span class="tex-font-style-it">non-increasing</span> (decrease or remained unchanged). It is possible that any of these two areas will be omitted. For example, the following sequences of block height meet this requirement:</p><ul> <li> <span class="tex-span">[1, 2, 2, 3, 4, 4, 3, 1]</span>; </li><li> <span class="tex-span">[1, 1]</span>; </li><li> <span class="tex-span">[2, 2, 1, 1]</span>; </li><li> <span class="tex-span">[1, 2, 3, 3, 2, 1]</span>. </li></ul><p>Suddenly, <span class="tex-span"><i>k</i></span> more requirements appeared. Each of the requirements has the form: "<span class="tex-span"><i>h</i>[<i>x</i><sub class="lower-index"><i>i</i></sub>]</span> <span class="tex-font-style-tt">sign</span><span class="tex-span"><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>h</i>[<i>y</i><sub class="lower-index"><i>i</i></sub>]</span>", where <span class="tex-span"><i>h</i>[<i>t</i>]</span> is the height of the <span class="tex-span"><i>t</i></span>-th block, and a <span class="tex-font-style-tt">sign</span><span class="tex-span"><sub class="lower-index"><i>i</i></sub></span> is one of the five possible signs: '<span class="tex-font-style-tt">=</span>' (equals), '<span class="tex-font-style-tt">&lt;</span>' (less than), '<span class="tex-font-style-tt">&gt;</span>' (more than), '<span class="tex-font-style-tt">&lt;=</span>' (less than or equals), '<span class="tex-font-style-tt">&gt;=</span>' (more than or equals). Thus, each of the <span class="tex-span"><i>k</i></span> additional requirements is given by a pair of indexes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i></span>) and sign <span class="tex-font-style-tt">sign</span><span class="tex-span"><sub class="lower-index"><i>i</i></sub></span>.</p><p>Find the number of possible ways to rearrange the blocks so that both the requirement about the shape of the mausoleum (see paragraph 3) and the <span class="tex-span"><i>k</i></span> additional requirements were met.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 35</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>) — the number of pairs of blocks and the number of additional requirements.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain listed additional requirements, one per line in the format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-tt">sign</span><span class="tex-span"><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i></span>), and the sign is on of the list of the five possible signs.</p></div><div class="output-specification"><p>Print the sought number of ways.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 35</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>) — the number of pairs of blocks and the number of additional requirements.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain listed additional requirements, one per line in the format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-tt">sign</span><span class="tex-span"><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i></span>), and the sign is on of the list of the five possible signs.</p>

## Output

<p>Print the sought number of ways.</p>





```input1
3 0

```




```input2
3 1
2 &gt; 3

```




```input3
4 1
3 = 6

```




```output1
9

```




```output2
1

```




```output3
3

```


