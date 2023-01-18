## Description

<div><p>On the way to Rio de Janeiro Ostap kills time playing with a grasshopper he took with him in a special box. Ostap builds a line of length <span class="tex-span"><i>n</i></span> such that some cells of this line are empty and some contain obstacles. Then, he places his grasshopper to one of the empty cells and a small insect in another empty cell. The grasshopper wants to eat the insect.</p><p>Ostap knows that grasshopper is able to jump to any empty cell that is <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span> cells away from the current (to the left or to the right). Note that it doesn't matter whether intermediate cells are empty or not as the grasshopper makes a jump over them. For example, if <span class="tex-span"><i>k</i> = 1</span> the grasshopper can jump to a neighboring cell only, and if <span class="tex-span"><i>k</i> = 2</span> the grasshopper can jump over a single cell.</p><p>Your goal is to determine whether there is a sequence of jumps such that grasshopper will get from his initial position to the cell with an insect.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>)&nbsp;— the number of cells in the line and the length of one grasshopper's jump.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> consisting of characters '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">T</span>'. Character '<span class="tex-font-style-tt">.</span>' means that the corresponding cell is empty, character '<span class="tex-font-style-tt">#</span>' means that the corresponding cell contains an obstacle and grasshopper can't jump there. Character '<span class="tex-font-style-tt">G</span>' means that the grasshopper starts at this position and, finally, '<span class="tex-font-style-tt">T</span>' means that the target insect is located at this cell. It's guaranteed that characters '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">T</span>' appear in this line <span class="tex-font-style-bf">exactly once</span>.</p></div><div class="output-specification"><p>If there exists a sequence of jumps (each jump of length <span class="tex-span"><i>k</i></span>), such that the grasshopper can get from his initial position to the cell with the insect, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the input. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>)&nbsp;— the number of cells in the line and the length of one grasshopper's jump.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> consisting of characters '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">T</span>'. Character '<span class="tex-font-style-tt">.</span>' means that the corresponding cell is empty, character '<span class="tex-font-style-tt">#</span>' means that the corresponding cell contains an obstacle and grasshopper can't jump there. Character '<span class="tex-font-style-tt">G</span>' means that the grasshopper starts at this position and, finally, '<span class="tex-font-style-tt">T</span>' means that the target insect is located at this cell. It's guaranteed that characters '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">T</span>' appear in this line <span class="tex-font-style-bf">exactly once</span>.</p>

## Output

<p>If there exists a sequence of jumps (each jump of length <span class="tex-span"><i>k</i></span>), such that the grasshopper can get from his initial position to the cell with the insect, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the input. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
5 2
#G#T#

```




```input2
6 1
T....G

```




```input3
7 3
T..#..G

```




```input4
6 2
..GT..

```




```output1
YES

```




```output2
YES

```




```output3
NO

```




```output4
NO

```



## Note

<p>In the first sample, the grasshopper can make one jump to the right in order to get from cell <span class="tex-span">2</span> to cell <span class="tex-span">4</span>.</p><p>In the second sample, the grasshopper is only able to jump to neighboring cells but the way to the insect is free&nbsp;— he can get there by jumping left <span class="tex-span">5</span> times.</p><p>In the third sample, the grasshopper can't make a single jump.</p><p>In the fourth sample, the grasshopper can only jump to the cells with odd indices, thus he won't be able to reach the insect.</p>
