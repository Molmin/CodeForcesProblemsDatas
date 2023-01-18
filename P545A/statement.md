## Description

<div><p>Little Susie, thanks to her older brother, likes to play with cars. Today she decided to set up a tournament between them. The process of a tournament is described in the next paragraph.</p><p>There are <span class="tex-span"><i>n</i></span> toy cars. Each pair collides. The result of a collision can be one of the following: no car turned over, one car turned over, both cars turned over. A car is good if it turned over in no collision. The results of the collisions are determined by an <span class="tex-span"><i>n</i> × <i>n</i></span> matrix <span class="tex-span"><i>А</i></span>: there is a number on the intersection of the <span class="tex-span"><i>і</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column that describes the result of the collision of the <span class="tex-span"><i>і</i></span>-th and the <span class="tex-span"><i>j</i></span>-th car: </p><ul> <li> <span class="tex-span"> - 1</span>: if this pair of cars never collided. <span class="tex-span"> - 1</span> occurs only on the main diagonal of the matrix. </li><li> <span class="tex-span">0</span>: if no car turned over during the collision. </li><li> <span class="tex-span">1</span>: if only the <span class="tex-span"><i>i</i></span>-th car turned over during the collision. </li><li> <span class="tex-span">2</span>: if only the <span class="tex-span"><i>j</i></span>-th car turned over during the collision. </li><li> <span class="tex-span">3</span>: if both cars turned over during the collision. </li></ul><p>Susie wants to find all the good cars. She quickly determined which cars are good. Can you cope with the task?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cars.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> space-separated integers that determine matrix <span class="tex-span"><i>A</i></span>. </p><p>It is guaranteed that on the main diagonal there are <span class="tex-span"> - 1</span>, and <span class="tex-span"> - 1</span> doesn't appear anywhere else in the matrix.</p><p>It is guaranteed that the input is correct, that is, if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 1</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 2</span>, if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 3</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 3</span>, and if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 0</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 0</span>.</p></div><div class="output-specification"><p>Print the number of good cars and in the next line print their space-separated indices in the increasing order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cars.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> space-separated integers that determine matrix <span class="tex-span"><i>A</i></span>. </p><p>It is guaranteed that on the main diagonal there are <span class="tex-span"> - 1</span>, and <span class="tex-span"> - 1</span> doesn't appear anywhere else in the matrix.</p><p>It is guaranteed that the input is correct, that is, if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 1</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 2</span>, if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 3</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 3</span>, and if <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = 0</span>, then <span class="tex-span"><i>A</i><sub class="lower-index"><i>ji</i></sub> = 0</span>.</p>

## Output

<p>Print the number of good cars and in the next line print their space-separated indices in the increasing order.</p>





```input1
3
-1 0 0
0 -1 1
0 2 -1

```




```input2
4
-1 3 3 3
3 -1 3 3
3 3 -1 3
3 3 3 -1

```




```output1
2
1 3
```




```output2
0

```


