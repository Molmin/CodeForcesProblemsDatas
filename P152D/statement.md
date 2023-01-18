## Description

<div><p>One day Vasya got hold of a sheet of checkered paper <span class="tex-span"><i>n</i> × <i>m</i></span> squares in size. Our Vasya adores geometrical figures, so he painted two rectangles on the paper. The rectangles' sides are parallel to the coordinates' axes, also the length of each side of each rectangle is no less than 3 squares and the sides are painted by the grid lines. The sides can also be part of the sheet of paper's edge. Then Vasya hatched all squares on the rectangles' <span class="tex-font-style-underline">frames</span>.</p><p>Let's define a rectangle's frame as the set of squares <span class="tex-font-style-bf">inside</span> the rectangle that share at least one side with its border.</p><p>A little later Vasya found a sheet of paper of exactly the same size and couldn't guess whether it is the same sheet of paper or a different one. So, he asked you to check whether the sheet of paper he had found contains two painted frames and nothing besides them.</p><p>Please note that the frames painted by Vasya can arbitrarily intersect, overlap or even completely coincide.</p><p>The coordinates on the sheet of paper are introduced in such a way that the <span class="tex-span"><i>X</i></span> axis goes from top to bottom, the <span class="tex-span"><i>x</i></span> coordinates of the squares' numbers take values from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the <span class="tex-span"><i>Y</i></span> axis goes from the left to the right and the <span class="tex-span"><i>y</i></span> coordinates of the squares' numbers take values from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the sizes of the sheet of paper Vasya found. Next <span class="tex-span"><i>n</i></span> lines, each consisting of <span class="tex-span"><i>m</i></span> symbols "<span class="tex-font-style-tt">.</span>" (dot) and "<span class="tex-font-style-tt">#</span>" (number sign), describe the found sheet of paper. The symbol "<span class="tex-font-style-tt">#</span>" represents a hatched square and the symbol "<span class="tex-font-style-tt">.</span>" represents a non-hatched square.</p></div><div class="output-specification"><p>In the first line print the single word "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", meaning whether it is true that the found sheet of paper has two frames painted on it. If the answer is positive, then print in the second line <span class="tex-span">4</span> integers: the coordinates of the upper left and lower right corners of the first frame. In the third line print <span class="tex-span">4</span> integers: the coordinates of the upper left and the lower right corners of the second frame. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the sizes of the sheet of paper Vasya found. Next <span class="tex-span"><i>n</i></span> lines, each consisting of <span class="tex-span"><i>m</i></span> symbols "<span class="tex-font-style-tt">.</span>" (dot) and "<span class="tex-font-style-tt">#</span>" (number sign), describe the found sheet of paper. The symbol "<span class="tex-font-style-tt">#</span>" represents a hatched square and the symbol "<span class="tex-font-style-tt">.</span>" represents a non-hatched square.</p>

## Output

<p>In the first line print the single word "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", meaning whether it is true that the found sheet of paper has two frames painted on it. If the answer is positive, then print in the second line <span class="tex-span">4</span> integers: the coordinates of the upper left and lower right corners of the first frame. In the third line print <span class="tex-span">4</span> integers: the coordinates of the upper left and the lower right corners of the second frame. If there are multiple answers, print any of them.</p>





```input1
4 5
#####
#.#.#
###.#
#####

```




```input2
5 6
...###
...###
#####.
#...#.
#####.

```




```output1
YES
1 1 3 3
1 1 4 5

```




```output2
NO

```



## Note

<p>In the first sample there are two frames on the picture. The first one is:</p><pre class="verbatim">###..<br>#.#..<br>###..<br>.....<br></pre><p>The second one is:</p><pre class="verbatim">#####<br>#...#<br>#...#<br>#####<br></pre><p>In the second sample the painted figures are not frames. Note that the height and width of valid frames is no less than 3.</p>
