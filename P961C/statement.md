## Description

<div><p>Magnus decided to play a classic chess game. Though what he saw in his locker shocked him! His favourite chessboard got broken into <span class="tex-span">4</span> pieces, each of size <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>n</i></span> is <span class="tex-font-style-bf">always odd</span>. And what's even worse, some squares were of wrong color. <span class="tex-span"><i>j</i></span>-th square of the <span class="tex-span"><i>i</i></span>-th row of <span class="tex-span"><i>k</i></span>-th piece of the board has color <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i>, <i>i</i>, <i>j</i></sub></span>; <span class="tex-span">1</span> being black and <span class="tex-span">0</span> being white. </p><p>Now Magnus wants to change color of some squares in such a way that he recolors minimum number of squares and obtained pieces form a valid chessboard. Every square has its color different to each of the neightbouring by side squares in a valid board. Its size should be <span class="tex-span">2<i>n</i></span> by <span class="tex-span">2<i>n</i></span>. You are allowed to move pieces but <span class="tex-font-style-bf">not allowed to rotate or flip them</span>.</p></div><div class="input-specification"><p>The first line contains <span class="tex-font-style-bf">odd</span> integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the size of all pieces of the board. </p><p>Then <span class="tex-span">4</span> segments follow, each describes one piece of the board. Each consists of <span class="tex-span"><i>n</i></span> lines of <span class="tex-span"><i>n</i></span> characters; <span class="tex-span"><i>j</i></span>-th one of <span class="tex-span"><i>i</i></span>-th line is equal to <span class="tex-font-style-tt">1</span> if the square is black initially and <span class="tex-font-style-tt">0</span> otherwise. Segments are separated by an empty line.</p></div><div class="output-specification"><p>Print one number — minimum number of squares Magnus should recolor to be able to obtain a valid chessboard.</p></div>

## Input

<p>The first line contains <span class="tex-font-style-bf">odd</span> integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the size of all pieces of the board. </p><p>Then <span class="tex-span">4</span> segments follow, each describes one piece of the board. Each consists of <span class="tex-span"><i>n</i></span> lines of <span class="tex-span"><i>n</i></span> characters; <span class="tex-span"><i>j</i></span>-th one of <span class="tex-span"><i>i</i></span>-th line is equal to <span class="tex-font-style-tt">1</span> if the square is black initially and <span class="tex-font-style-tt">0</span> otherwise. Segments are separated by an empty line.</p>

## Output

<p>Print one number — minimum number of squares Magnus should recolor to be able to obtain a valid chessboard.</p>





```input1
1
0

0

1

0

```




```input2
3
101
010
101

101
000
101

010
101
011

010
101
010

```




```output1
1

```




```output2
2

```


