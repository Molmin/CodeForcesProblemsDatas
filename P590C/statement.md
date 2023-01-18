## Description

<div><p>The famous global economic crisis is approaching rapidly, so the states of Berman, Berance and Bertaly formed an alliance and allowed the residents of all member states to freely pass through the territory of any of them. In addition, it was decided that a road between the states should be built to guarantee so that one could any point of any country can be reached from any point of any other State.</p><p>Since roads are always expensive, the governments of the states of the newly formed alliance asked you to help them assess the costs. To do this, you have been issued a map that can be represented as a rectangle table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Any cell of the map either belongs to one of three states, or is an area where it is allowed to build a road, or is an area where the construction of the road is not allowed. A cell is called <span class="tex-font-style-it">passable</span>, if it belongs to one of the states, or the road was built in this cell. From any passable cells you can move up, down, right and left, if the cell that corresponds to the movement exists and is passable.</p><p>Your task is to construct a road inside a minimum number of cells, so that it would be possible to get from any cell of any state to any cell of any other state using only passable cells.</p><p>It is guaranteed that initially it is possible to reach any cell of any state from any cell of this state, moving only along its cells. It is also guaranteed that for any state there is at least one cell that belongs to it.</p></div><div class="input-specification"><p>The first line of the input contains the dimensions of the map <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and columns respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters, describing the rows of the map. Digits from <span class="tex-span">1</span> to <span class="tex-span">3</span> represent the accessory to the corresponding state. The character '<span class="tex-font-style-tt">.</span>' corresponds to the cell where it is allowed to build a road and the character '<span class="tex-font-style-tt">#</span>' means no construction is allowed in this cell.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of cells you need to build a road inside in order to connect all the cells of all states. If such a goal is unachievable, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input contains the dimensions of the map <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and columns respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters, describing the rows of the map. Digits from <span class="tex-span">1</span> to <span class="tex-span">3</span> represent the accessory to the corresponding state. The character '<span class="tex-font-style-tt">.</span>' corresponds to the cell where it is allowed to build a road and the character '<span class="tex-font-style-tt">#</span>' means no construction is allowed in this cell.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of cells you need to build a road inside in order to connect all the cells of all states. If such a goal is unachievable, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 5
11..2
#..22
#.323
.#333
```




```input2
1 5
1#2#3

```




```output1
2
```




```output2
-1

```


