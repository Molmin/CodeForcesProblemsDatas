## Description

<div><p>Andrew loves the sea. That's why, at the height of the summer season, he decided to go to the beach, taking a sunbed with him to sunbathe.</p><p>The beach is a rectangular field with $n$ rows and $m$ columns. Some cells of the beach are free, some have roads, stones, shops and other non-movable objects. Some of two adjacent along the side cells can have sunbeds located either horizontally or vertically.</p><p>Andrew hopes to put his sunbed somewhere, but that's a bad luck, there may no longer be free places for him! That's why Andrew asked you to help him to find a free place for his sunbed. Andrew's sunbed also should be places on two adjacent cells. </p><p>If there are no two adjacent free cells, then in order to free some place for a sunbed, you will have to disturb other tourists. You can do the following actions:</p><ul> <li> Come to some sunbed and, after causing $p$ units of discomfort to its owner, lift the sunbed by one of its sides and rotate it by $90$ degrees. One half of the sunbed must remain in the same cell and another half of the sunbed must move to the free cell. At the same time, anything could be on the way of a sunbed during the rotation .<center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://3wkkp1qg.png" style="max-width: 100.0%;max-height: 100.0%;" width="192px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://U0t8FiCS.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://Kra3nvDh.png" style="max-width: 100.0%;max-height: 100.0%;" width="192px"></td></tr></tbody></table>  <span class="tex-font-size-small">Rotation of the sunbed by $90$ degrees around cell $(1, 2)$.</span> </center></li><li> Come to some sunbed and, after causing $q$ units of discomfort to its owner, shift the sunbed along its long side by one cell. One half of the sunbed must move to the place of another, and another&nbsp;— to the free cell.<center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://zraU7ljD.png" style="max-width: 100.0%;max-height: 100.0%;" width="192px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://YDs60cnQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://IP8sqpjc.png" style="max-width: 100.0%;max-height: 100.0%;" width="192px"></td></tr></tbody></table>  <span class="tex-font-size-small">Shift of the sunbed by one cell to the right.</span> </center></li></ul><p>In any moment each sunbed occupies two adjacent free cells. You cannot move more than one sunbed at a time.</p><p>Help Andrew to free a space for his sunbed, causing the minimum possible number of units of discomfort to other tourists, or detect that it is impossible.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 300\,000$, $1 \le n \cdot m \le 300\,000$)&nbsp;— the number of rows and columns in rectangle.</p><p>The second line contains two integers $p$ and $q$ ($1 \le p, q \le 10^9$)&nbsp;— the number of units of discomfort caused by rotation and shift of a sunbed, respectively.</p><p>Each of the following $n$ lines contains $m$ characters, describing cells of the rectangle. Each lines consists of characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>", denoting the type of the cell. Characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>" and "<span class="tex-font-style-tt">U</span>" denote a half of a sunbed placed in the cell&nbsp;— left, right, bottom and top half, respectively. Character "<span class="tex-font-style-tt">.</span>" denotes a free cell and character "<span class="tex-font-style-tt">#</span>"&nbsp;— a cell, occupied by some non-movable object.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum possible number of units of discomfort, caused to other tourists, to free a space for a sunbed. If it is impossible to free a space for a sunbed, print $-1$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 300\,000$, $1 \le n \cdot m \le 300\,000$)&nbsp;— the number of rows and columns in rectangle.</p><p>The second line contains two integers $p$ and $q$ ($1 \le p, q \le 10^9$)&nbsp;— the number of units of discomfort caused by rotation and shift of a sunbed, respectively.</p><p>Each of the following $n$ lines contains $m$ characters, describing cells of the rectangle. Each lines consists of characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>", denoting the type of the cell. Characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>" and "<span class="tex-font-style-tt">U</span>" denote a half of a sunbed placed in the cell&nbsp;— left, right, bottom and top half, respectively. Character "<span class="tex-font-style-tt">.</span>" denotes a free cell and character "<span class="tex-font-style-tt">#</span>"&nbsp;— a cell, occupied by some non-movable object.</p>

## Output

<p>Print one integer&nbsp;— the minimum possible number of units of discomfort, caused to other tourists, to free a space for a sunbed. If it is impossible to free a space for a sunbed, print $-1$.</p>





```input1|
2 5
5 2
.LR##
##LR.
```




```input2|
2 3
4 5
LR.
#.#
```




```input3|
4 3
10 10
.LR
###
UU#
DD.
```




```input4|
3 6
10 7
.U##.#
#DLR##
.##LR.
```




```output1
4
```




```output2
-1
```




```output3
-1
```




```output4
24
```



## Note

<p>In the first example we can shift upper sunbed to the left and lower sunbed&nbsp;— to the right. Andrew will be able to put his sunbed vertically in the middle of the beach. We well cause $2 + 2 = 4$ units of discomfort. It is easy to prove that it is an optimal answer. </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://fdUfBcg0.png" style="max-width: 100.0%;max-height: 100.0%;" width="240px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://IoFLXR5m.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://WGncE7PD.png" style="max-width: 100.0%;max-height: 100.0%;" width="240px"></td></tr></tbody></table>  <span class="tex-font-size-small">Optimal strategy in the first example (Andrew's sunbed is colored white).</span> </center> In the second example it is impossible to free a space for Andrew's sunbed. All possible states of the beach after any rotates and shifts are illustrated in the problem statement.
