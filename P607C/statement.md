## Description

<div><p>In the spirit of the holidays, Saitama has given Genos two grid paths of length <span class="tex-span"><i>n</i></span> (a weird gift even by Saitama's standards). A grid path is an ordered sequence of neighbouring squares in an infinite grid. Two squares are neighbouring if they share a side.</p><p>One example of a grid path is <span class="tex-span">(0, 0) → (0, 1) → (0, 2) → (1, 2) → (1, 1) → (0, 1) → ( - 1, 1)</span>. Note that squares in this sequence might be repeated, i.e. path has self intersections.</p><p>Movement within a grid path is restricted to adjacent squares within the sequence. That is, from the <span class="tex-span"><i>i</i></span>-th square, one can <span class="tex-font-style-bf">only move</span> to the <span class="tex-span">(<i>i</i> - 1)</span>-th or <span class="tex-span">(<i>i</i> + 1)</span>-th squares of this path. Note that there is only a single valid move from the first and last squares of a grid path. Also note, that even if there is some <span class="tex-span"><i>j</i></span>-th square of the path that coincides with the <span class="tex-span"><i>i</i></span>-th square, only moves to <span class="tex-span">(<i>i</i> - 1)</span>-th and <span class="tex-span">(<i>i</i> + 1)</span>-th squares are available. For example, from the second square in the above sequence, one can only move to either the first or third squares.</p><p>To ensure that movement is not ambiguous, the two grid paths will not have an alternating sequence of three squares. For example, a contiguous subsequence <span class="tex-span">(0, 0) → (0, 1) → (0, 0)</span> <span class="tex-font-style-bf">cannot occur</span> in a valid grid path.</p><p>One marble is placed on the first square of each grid path. Genos wants to get both marbles to the last square of each grid path. However, there is a catch. Whenever he moves one marble, the other marble will copy its movement if possible. For instance, if one marble moves east, then the other marble will <span class="tex-font-style-it">try</span> and move east as well. By <span class="tex-font-style-it">try</span>, we mean if moving east is a valid move, then the marble will move east.</p><p>Moving north increases the second coordinate by <span class="tex-span">1</span>, while moving south decreases it by <span class="tex-span">1</span>. Similarly, moving east increases first coordinate by <span class="tex-span">1</span>, while moving west decreases it.</p><p>Given these two valid grid paths, Genos wants to know if it is possible to move both marbles to the ends of their respective paths. That is, if it is possible to move the marbles such that both marbles rest on the last square of their respective paths.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the length of the paths.</p><p>The second line of the input contains a string consisting of <span class="tex-span"><i>n</i> - 1</span> characters (each of which is either '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">W</span>')&nbsp;— the first grid path. The characters can be thought of as the sequence of moves needed to traverse the grid path. For example, the example path in the problem statement can be expressed by the string "<span class="tex-font-style-tt">NNESWW</span>".</p><p>The third line of the input contains a string of <span class="tex-span"><i>n</i> - 1</span> characters (each of which is either '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">W</span>')&nbsp;— the second grid path.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible for both marbles to be at the end position at the same time. Print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. In both cases, the answer is case-insensitive.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the length of the paths.</p><p>The second line of the input contains a string consisting of <span class="tex-span"><i>n</i> - 1</span> characters (each of which is either '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">W</span>')&nbsp;— the first grid path. The characters can be thought of as the sequence of moves needed to traverse the grid path. For example, the example path in the problem statement can be expressed by the string "<span class="tex-font-style-tt">NNESWW</span>".</p><p>The third line of the input contains a string of <span class="tex-span"><i>n</i> - 1</span> characters (each of which is either '<span class="tex-font-style-tt">N</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">W</span>')&nbsp;— the second grid path.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible for both marbles to be at the end position at the same time. Print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. In both cases, the answer is case-insensitive.</p>





```input1
7
NNESWW
SWSWSW

```




```input2
3
NN
SS

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, the first grid path is the one described in the statement. Moreover, the following sequence of moves will get both marbles to the end: <span class="tex-font-style-tt">NNESWWSWSW</span>.</p><p>In the second sample, no sequence of moves can get both marbles to the end.</p>
