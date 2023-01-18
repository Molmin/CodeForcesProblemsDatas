## Description

<div><p>Joe has been hurt on the Internet. Now he is storming around the house, destroying everything in his path.</p><p>Joe's house has <span class="tex-span"><i>n</i></span> floors, each floor is a segment of <span class="tex-span"><i>m</i></span> cells. Each cell either contains nothing (it is an empty cell), or has a brick or a concrete wall (always something one of three). It is believed that each floor is surrounded by a concrete wall on the left and on the right.</p><p>Now Joe is on the <span class="tex-span"><i>n</i></span>-th floor and in the first cell, counting from left to right. At each moment of time, Joe has the direction of his gaze, to the right or to the left (always one direction of the two). Initially, Joe looks to the right.</p><p>Joe moves by a particular algorithm. Every second he makes one of the following actions: </p><ul> <li> If the cell directly under Joe is empty, then Joe falls down. That is, he moves to this cell, the gaze direction is preserved. </li><li> Otherwise consider the next cell in the current direction of the gaze. <ul> <li> If the cell is empty, then Joe moves into it, the gaze direction is preserved. </li><li> If this cell has bricks, then Joe breaks them with his forehead (the cell becomes empty), and changes the direction of his gaze to the opposite. </li><li> If this cell has a concrete wall, then Joe just changes the direction of his gaze to the opposite (concrete can withstand any number of forehead hits). </li></ul> </li></ul><p>Joe calms down as soon as he reaches <span class="tex-font-style-bf">any</span> cell of the first floor.</p><p>The figure below shows an example Joe's movements around the house.</p><center> <img class="tex-graphics" src="file://ezTUXHFr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Determine how many seconds Joe will need to calm down.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of Joe's house. The <span class="tex-span"><i>i</i></span>-th of these lines contains the description of the <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span>-th floor of the house — a line that consists of <span class="tex-span"><i>m</i></span> characters: "<span class="tex-font-style-tt">.</span>" means an empty cell, "<span class="tex-font-style-tt">+</span>" means bricks and "<span class="tex-font-style-tt">#</span>" means a concrete wall.</p><p>It is guaranteed that the first cell of the <span class="tex-span"><i>n</i></span>-th floor is empty.</p></div><div class="output-specification"><p>Print a single number — the number of seconds Joe needs to reach the first floor; or else, print word "<span class="tex-font-style-tt">Never</span>" (without the quotes), if it can never happen.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of Joe's house. The <span class="tex-span"><i>i</i></span>-th of these lines contains the description of the <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span>-th floor of the house — a line that consists of <span class="tex-span"><i>m</i></span> characters: "<span class="tex-font-style-tt">.</span>" means an empty cell, "<span class="tex-font-style-tt">+</span>" means bricks and "<span class="tex-font-style-tt">#</span>" means a concrete wall.</p><p>It is guaranteed that the first cell of the <span class="tex-span"><i>n</i></span>-th floor is empty.</p>

## Output

<p>Print a single number — the number of seconds Joe needs to reach the first floor; or else, print word "<span class="tex-font-style-tt">Never</span>" (without the quotes), if it can never happen.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 5
..+.#
#+..+
+.#+.

```




```input2
4 10
...+.##+.+
+#++..+++#
++.#++++..
.+##.++#.+

```




```input3
2 2
..
++

```




```output1
14
```




```output2
42

```




```output3
Never
```


