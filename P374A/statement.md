## Description

<div><p>Dima and Inna are doing so great! At the moment, Inna is sitting on the magic lawn playing with a pink pony. Dima wanted to play too. He brought an <span class="tex-span"><i>n</i> × <i>m</i></span> chessboard, a very tasty candy and two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>Dima put the chessboard in front of Inna and placed the candy in position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> on the board. The boy said he would give the candy if it reaches one of the corner cells of the board. He's got one more condition. There can only be actions of the following types:</p><ul> <li> move the candy from position <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on the board to position <span class="tex-span">(<i>x</i> - <i>a</i>, <i>y</i> - <i>b</i>)</span>; </li><li> move the candy from position <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on the board to position <span class="tex-span">(<i>x</i> + <i>a</i>, <i>y</i> - <i>b</i>)</span>; </li><li> move the candy from position <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on the board to position <span class="tex-span">(<i>x</i> - <i>a</i>, <i>y</i> + <i>b</i>)</span>; </li><li> move the candy from position <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on the board to position <span class="tex-span">(<i>x</i> + <i>a</i>, <i>y</i> + <i>b</i>)</span>. </li></ul><p>Naturally, Dima doesn't allow to move the candy beyond the chessboard borders.</p><p>Inna and the pony started shifting the candy around the board. They wonder what is the minimum number of allowed actions that they need to perform to move the candy from the initial position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> to one of the chessboard corners. Help them cope with the task! </p></div><div class="input-specification"><p>The first line of the input contains six integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>i</i>, <i>j</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;1 ≤ <i>i</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>j</i> ≤ <i>m</i>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>You can assume that the chessboard rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom and the columns are numbered from 1 to <span class="tex-span"><i>m</i></span> from left to right. Position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> in the statement is a chessboard cell on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. You can consider that the corners are: <span class="tex-span">(1, <i>m</i>)</span>, <span class="tex-span">(<i>n</i>, 1)</span>, <span class="tex-span">(<i>n</i>, <i>m</i>)</span>, <span class="tex-span">(1, 1)</span>.</p></div><div class="output-specification"><p>In a single line print a single integer — the minimum number of moves needed to get the candy.</p><p>If Inna and the pony cannot get the candy playing by Dima's rules, print on a single line "<span class="tex-font-style-tt">Poor Inna and pony!</span>" without the quotes.</p></div>

## Input

<p>The first line of the input contains six integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>i</i>, <i>j</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;1 ≤ <i>i</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>j</i> ≤ <i>m</i>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>You can assume that the chessboard rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom and the columns are numbered from 1 to <span class="tex-span"><i>m</i></span> from left to right. Position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> in the statement is a chessboard cell on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. You can consider that the corners are: <span class="tex-span">(1, <i>m</i>)</span>, <span class="tex-span">(<i>n</i>, 1)</span>, <span class="tex-span">(<i>n</i>, <i>m</i>)</span>, <span class="tex-span">(1, 1)</span>.</p>

## Output

<p>In a single line print a single integer — the minimum number of moves needed to get the candy.</p><p>If Inna and the pony cannot get the candy playing by Dima's rules, print on a single line "<span class="tex-font-style-tt">Poor Inna and pony!</span>" without the quotes.</p>





```input1
5 7 1 3 2 2

```




```input2
5 5 2 3 1 1

```




```output1
2

```




```output2
Poor Inna and pony!

```



## Note

<p>Note to sample 1:</p><p>Inna and the pony can move the candy to position <span class="tex-span">(1 + 2, 3 + 2) = (3, 5)</span>, from there they can move it to positions <span class="tex-span">(3 - 2, 5 + 2) = (1, 7)</span> and <span class="tex-span">(3 + 2, 5 + 2) = (5, 7)</span>. These positions correspond to the corner squares of the chess board. Thus, the answer to the test sample equals two.</p>
