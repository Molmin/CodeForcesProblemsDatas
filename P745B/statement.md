## Description

<div><p>Hongcow likes solving puzzles.</p><p>One day, Hongcow finds two identical puzzle pieces, with the instructions "make a rectangle" next to them. The pieces can be described by an <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>m</i></span> grid of characters, where the character '<span class="tex-font-style-tt">X</span>' denotes a part of the puzzle and '<span class="tex-font-style-tt">.</span>' denotes an empty part of the grid. It is guaranteed that the puzzle pieces are one 4-connected piece. See the input format and samples for the exact details on how a jigsaw piece will be specified.</p><p>The puzzle pieces are very heavy, so Hongcow <span class="tex-font-style-bf">cannot rotate or flip</span> the puzzle pieces. However, he is allowed to move them in any directions. The puzzle pieces also <span class="tex-font-style-bf">cannot overlap</span>.</p><p>You are given as input the description of one of the pieces. Determine if it is possible to make a rectangle from two identical copies of the given input. The rectangle should be solid, i.e. there should be no empty holes inside it or on its border. Keep in mind that Hongcow is not allowed to flip or rotate pieces and they cannot overlap, i.e. no two '<span class="tex-font-style-tt">X</span>' from different pieces can share the same position.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>), the dimensions of the puzzle piece.</p><p>The next <span class="tex-span"><i>n</i></span> lines will describe the jigsaw piece. Each line will have length <span class="tex-span"><i>m</i></span> and will consist of characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">X</span>' only. '<span class="tex-font-style-tt">X</span>' corresponds to a part of the puzzle piece, '<span class="tex-font-style-tt">.</span>' is an empty space.</p><p>It is guaranteed there is at least one '<span class="tex-font-style-tt">X</span>' character in the input and that the '<span class="tex-font-style-tt">X</span>' characters form a 4-connected region.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" if it is possible for Hongcow to make a rectangle. Output "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>), the dimensions of the puzzle piece.</p><p>The next <span class="tex-span"><i>n</i></span> lines will describe the jigsaw piece. Each line will have length <span class="tex-span"><i>m</i></span> and will consist of characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">X</span>' only. '<span class="tex-font-style-tt">X</span>' corresponds to a part of the puzzle piece, '<span class="tex-font-style-tt">.</span>' is an empty space.</p><p>It is guaranteed there is at least one '<span class="tex-font-style-tt">X</span>' character in the input and that the '<span class="tex-font-style-tt">X</span>' characters form a 4-connected region.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" if it is possible for Hongcow to make a rectangle. Output "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
2 3
XXX
XXX

```




```input2
2 2
.X
XX

```




```input3
5 5
.....
..X..
.....
.....
.....

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>For the first sample, one example of a rectangle we can form is as follows </p><pre class="verbatim"><br>111222<br>111222<br></pre><p>For the second sample, it is impossible to put two of those pieces without rotating or flipping to form a rectangle.</p><p>In the third sample, we can shift the first tile by one to the right, and then compose the following rectangle: </p><pre class="verbatim"><br>.....<br>..XX.<br>.....<br>.....<br>.....<br></pre>
