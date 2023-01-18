## Description

<div><p>Bob is a farmer. He has a large pasture with many sheep. Recently, he has lost some of them due to wolf attacks. He thus decided to place some shepherd dogs in such a way that all his sheep are protected.</p><p>The pasture is a rectangle consisting of <span class="tex-span"><i>R</i> × <i>C</i></span> cells. Each cell is either empty, contains a sheep, a wolf or a dog. Sheep and dogs always stay in place, but wolves can roam freely around the pasture, by repeatedly moving to the left, right, up or down to a neighboring cell. When a wolf enters a cell with a sheep, it consumes it. However, no wolf can enter a cell with a dog.</p><p>Initially there are no dogs. Place dogs onto the pasture in such a way that no wolf can reach any sheep, or determine that it is impossible. Note that since you have many dogs, you do <span class="tex-font-style-bf">not</span> need to minimize their number. </p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ 500</span>) and <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 500</span>), denoting the number of rows and the numbers of columns respectively.</p><p>Each of the following <span class="tex-span"><i>R</i></span> lines is a string consisting of exactly <span class="tex-span"><i>C</i></span> characters, representing one row of the pasture. Here, '<span class="tex-font-style-tt">S</span>' means a sheep, '<span class="tex-font-style-tt">W</span>' a wolf and '<span class="tex-font-style-tt">.</span>' an empty cell.</p></div><div class="output-specification"><p>If it is impossible to protect all sheep, output a single line with the word "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, output a line with the word "<span class="tex-font-style-tt">Yes</span>". Then print <span class="tex-span"><i>R</i></span> lines, representing the pasture after placing dogs. Again, '<span class="tex-font-style-tt">S</span>' means a sheep, '<span class="tex-font-style-tt">W</span>' a wolf, '<span class="tex-font-style-tt">D</span>' is a dog and '<span class="tex-font-style-tt">.</span>' an empty space. You are not allowed to move, remove or add a sheep or a wolf.</p><p>If there are multiple solutions, you may print any of them. You don't have to minimize the number of dogs.</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ 500</span>) and <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 500</span>), denoting the number of rows and the numbers of columns respectively.</p><p>Each of the following <span class="tex-span"><i>R</i></span> lines is a string consisting of exactly <span class="tex-span"><i>C</i></span> characters, representing one row of the pasture. Here, '<span class="tex-font-style-tt">S</span>' means a sheep, '<span class="tex-font-style-tt">W</span>' a wolf and '<span class="tex-font-style-tt">.</span>' an empty cell.</p>

## Output

<p>If it is impossible to protect all sheep, output a single line with the word "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, output a line with the word "<span class="tex-font-style-tt">Yes</span>". Then print <span class="tex-span"><i>R</i></span> lines, representing the pasture after placing dogs. Again, '<span class="tex-font-style-tt">S</span>' means a sheep, '<span class="tex-font-style-tt">W</span>' a wolf, '<span class="tex-font-style-tt">D</span>' is a dog and '<span class="tex-font-style-tt">.</span>' an empty space. You are not allowed to move, remove or add a sheep or a wolf.</p><p>If there are multiple solutions, you may print any of them. You don't have to minimize the number of dogs.</p>





```input1
6 6
..S...
..S.W.
.S....
..W...
...W..
......

```




```input2
1 2
SW

```




```input3
5 5
.S...
...S.
S....
...S.
.S...

```




```output1
Yes
..SD..
..SDW.
.SD...
.DW...
DD.W..
......

```




```output2
No

```




```output3
Yes
.S...
...S.
S.D..
...S.
.S...

```



## Note

<p>In the first example, we can split the pasture into two halves, one containing wolves and one containing sheep. Note that the sheep at (2,1) is safe, as wolves cannot move diagonally.</p><p>In the second example, there are no empty spots to put dogs that would guard the lone sheep.</p><p>In the third example, there are no wolves, so the task is very easy. We put a dog in the center to observe the peacefulness of the meadow, but the solution would be correct even without him.</p>
