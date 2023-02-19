## Description

<div><p>The Robot is in a rectangular maze of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell of the maze is either empty or occupied by an obstacle. The Robot can move between neighboring cells on the side left (the symbol "<span class="tex-font-style-tt">L</span>"), right (the symbol "<span class="tex-font-style-tt">R</span>"), up (the symbol "<span class="tex-font-style-tt">U</span>") or down (the symbol "<span class="tex-font-style-tt">D</span>"). The Robot can move to the cell only if it is empty. Initially, the Robot is in the empty cell.</p><p>Your task is to find <span class="tex-font-style-bf">lexicographically minimal</span> Robot's cycle with length <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span>, which begins and ends in the cell where the Robot was initially. It is allowed to the Robot to visit any cell many times (including starting).</p><p>Consider that Robot's way is given as a line which consists of symbols "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">U</span>" and "<span class="tex-font-style-tt">D</span>". For example, if firstly the Robot goes down, then left, then right and up, it means that his way is written as "<span class="tex-font-style-tt">DLRU</span>".</p><p>In this task you <span class="tex-font-style-bf">don't need</span> to minimize the length of the way. Find the minimum lexicographical (in alphabet order as in the dictionary) line which satisfies requirements above.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — the size of the maze and the length of the cycle. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols — the description of the maze. If the symbol equals to "<span class="tex-font-style-tt">.</span>" the current cell is empty. If the symbol equals to "<span class="tex-font-style-tt">*</span>" the current cell is occupied by an obstacle. If the symbol equals to "<span class="tex-font-style-tt">X</span>" then initially the Robot is in this cell and it is empty. It is guaranteed that the symbol "<span class="tex-font-style-tt">X</span>" is found in the maze exactly once. </p></div><div class="output-specification"><p>Print the lexicographically minimum Robot's way with the length exactly <span class="tex-span"><i>k</i></span>, which starts and ends in the cell where initially Robot is. If there is no such way, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>"(without quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — the size of the maze and the length of the cycle. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols — the description of the maze. If the symbol equals to "<span class="tex-font-style-tt">.</span>" the current cell is empty. If the symbol equals to "<span class="tex-font-style-tt">*</span>" the current cell is occupied by an obstacle. If the symbol equals to "<span class="tex-font-style-tt">X</span>" then initially the Robot is in this cell and it is empty. It is guaranteed that the symbol "<span class="tex-font-style-tt">X</span>" is found in the maze exactly once. </p>

## Output

<p>Print the lexicographically minimum Robot's way with the length exactly <span class="tex-span"><i>k</i></span>, which starts and ends in the cell where initially Robot is. If there is no such way, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>"(without quotes).</p>





```input1
2 3 2
.**
X..

```




```input2
5 6 14
..***.
*...X.
..*...
..*.**
....*.

```




```input3
3 3 4
***
*X*
***

```




```output1
RL

```




```output2
DLDDLLLRRRUURU

```




```output3
IMPOSSIBLE

```



## Note

<p>In the first sample two cyclic ways for the Robot with the length <span class="tex-span">2</span> exist — "<span class="tex-font-style-tt">UD</span>" and "<span class="tex-font-style-tt">RL</span>". The second cycle is lexicographically less. </p><p>In the second sample the Robot should move in the following way: down, left, down, down, left, left, left, right, right, right, up, up, right, up. </p><p>In the third sample the Robot can't move to the neighboring cells, because they are occupied by obstacles.</p>
