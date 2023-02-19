## Description

<div><p>You are playing the game "Arranging The Sheep". The goal of this game is to make the sheep line up. The level in the game is described by a string of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' (empty space) and '<span class="tex-font-style-tt">*</span>' (sheep). In one move, you can move any sheep one square to the left or one square to the right, if the corresponding square <span class="tex-font-style-bf">exists and is empty</span>. The game ends as soon as the sheep are lined up, that is, there should be no empty cells between any sheep.</p><p>For example, if $n=6$ and the level is described by the string "<span class="tex-font-style-tt">**.*..</span>", then the following game scenario is possible: </p><ul> <li> the sheep at the $4$ position moves to the right, the state of the level: "<span class="tex-font-style-tt">**..*.</span>"; </li><li> the sheep at the $2$ position moves to the right, the state of the level: "<span class="tex-font-style-tt">*.*.*.</span>"; </li><li> the sheep at the $1$ position moves to the right, the state of the level: "<span class="tex-font-style-tt">.**.*.</span>"; </li><li> the sheep at the $3$ position moves to the right, the state of the level: "<span class="tex-font-style-tt">.*.**.</span>"; </li><li> the sheep at the $2$ position moves to the right, the state of the level: "<span class="tex-font-style-tt">..***.</span>"; </li><li> the sheep are lined up and the game ends. </li></ul><p>For a given level, determine the minimum number of moves you need to make to complete the level.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^6$).</p><p>The second line of each test case contains a string of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' (empty space) and '<span class="tex-font-style-tt">*</span>' (sheep)&nbsp;— the description of the level.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case output the minimum number of moves you need to make to complete the level.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^6$).</p><p>The second line of each test case contains a string of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' (empty space) and '<span class="tex-font-style-tt">*</span>' (sheep)&nbsp;— the description of the level.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case output the minimum number of moves you need to make to complete the level.</p>





```input1
5
6
**.*..
5
*****
3
.*.
3
...
10
*.*...*.**
```




```output1
1
0
0
0
9
```


