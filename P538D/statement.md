## Description

<div><p>Igor has been into chess for a long time and now he is sick of the game by the ordinary rules. He is going to think of new rules of the game and become world famous.</p><p>Igor's chessboard is a square of size <span class="tex-span"><i>n</i> × <i>n</i></span> cells. Igor decided that simple rules guarantee success, that's why his game will have only one type of pieces. Besides, all pieces in his game are of the same color. The possible moves of a piece are described by a set of <span class="tex-font-style-it">shift vectors</span>. The next passage contains a formal description of available moves.</p><p>Let the rows of the board be numbered from top to bottom and the columns be numbered from left to right from 1 to <span class="tex-span"><i>n</i></span>. Let's assign to each square a pair of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span>&nbsp;— the number of the corresponding column and row. Each of the possible moves of the piece is defined by a pair of integers <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span>; using this move, the piece moves from the field <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to the field <span class="tex-span">(<i>x</i> + <i>dx</i>, <i>y</i> + <i>dy</i>)</span>. You can perform the move if the cell <span class="tex-span">(<i>x</i> + <i>dx</i>, <i>y</i> + <i>dy</i>)</span> is within the boundaries of the board and doesn't contain another piece. Pieces that stand on the cells other than <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>x</i> + <i>dx</i>, <i>y</i> + <i>dy</i>)</span> are not important when considering the possibility of making the given move (for example, like when a knight moves in usual chess).</p><p>Igor offers you to find out what moves his chess piece can make. He placed several pieces on the board and for each unoccupied square he told you whether it is attacked by any present piece (i.e. whether some of the pieces on the field can move to that cell). Restore a possible set of shift vectors of the piece, or else determine that Igor has made a mistake and such situation is impossible for any set of shift vectors.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> characters each describing the position offered by Igor. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string can have the following values:</p><ul><li> <span class="tex-font-style-tt">o</span> — in this case the field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is occupied by a piece and the field may or may not be attacked by some other piece;</li><li> <span class="tex-font-style-tt">x</span> — in this case field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is attacked by some piece;</li><li> <span class="tex-font-style-tt">.</span> — in this case field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> isn't attacked by any piece.</li></ul><p>It is guaranteed that there is at least one piece on the board.</p></div><div class="output-specification"><p>If there is a valid set of moves, in the first line print a single word '<span class="tex-font-style-tt">YES</span>' (without the quotes). Next, print the description of the set of moves of a piece in the form of a <span class="tex-span">(2<i>n</i> - 1) × (2<i>n</i> - 1)</span> board, the center of the board has a piece and symbols '<span class="tex-font-style-tt">x</span>' mark cells that are attacked by it, in a format similar to the input. See examples of the output for a full understanding of the format. If there are several possible answers, print any of them.</p><p>If a valid set of moves does not exist, print a single word '<span class="tex-font-style-tt">NO</span>'.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> characters each describing the position offered by Igor. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string can have the following values:</p><ul><li> <span class="tex-font-style-tt">o</span> — in this case the field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is occupied by a piece and the field may or may not be attacked by some other piece;</li><li> <span class="tex-font-style-tt">x</span> — in this case field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is attacked by some piece;</li><li> <span class="tex-font-style-tt">.</span> — in this case field <span class="tex-span">(<i>i</i>, <i>j</i>)</span> isn't attacked by any piece.</li></ul><p>It is guaranteed that there is at least one piece on the board.</p>

## Output

<p>If there is a valid set of moves, in the first line print a single word '<span class="tex-font-style-tt">YES</span>' (without the quotes). Next, print the description of the set of moves of a piece in the form of a <span class="tex-span">(2<i>n</i> - 1) × (2<i>n</i> - 1)</span> board, the center of the board has a piece and symbols '<span class="tex-font-style-tt">x</span>' mark cells that are attacked by it, in a format similar to the input. See examples of the output for a full understanding of the format. If there are several possible answers, print any of them.</p><p>If a valid set of moves does not exist, print a single word '<span class="tex-font-style-tt">NO</span>'.</p>





```input1
5
oxxxx
x...x
x...x
x...x
xxxxo

```




```input2
6
.x.x..
x.x.x.
.xo..x
x..ox.
.x.x.x
..x.x.

```




```input3
3
o.x
oxx
o.x

```




```output1
YES
....x....
....x....
....x....
....x....
xxxxoxxxx
....x....
....x....
....x....
....x....

```




```output2
YES
...........
...........
...........
....x.x....
...x...x...
.....o.....
...x...x...
....x.x....
...........
...........
...........

```




```output3
NO

```



## Note

<p>In the first sample test the piece is a usual chess rook, and in the second sample test the piece is a usual chess knight.</p>
