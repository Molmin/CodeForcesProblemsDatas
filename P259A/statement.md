## Description

<div><p>The Little Elephant loves chess very much. </p><p>One day the Little Elephant and his friend decided to play chess. They've got the chess pieces but the board is a problem. They've got an <span class="tex-span">8 × 8</span> checkered board, each square is painted either black or white. The Little Elephant and his friend know that a <span class="tex-font-style-it">proper chessboard</span> doesn't have any side-adjacent cells with the same color and the upper left cell is white. To play chess, they want to make the board they have a proper chessboard. For that the friends can choose any row of the board and cyclically shift the cells of the chosen row, that is, put the last (rightmost) square on the first place in the row and shift the others one position to the right. You can run the described operation <span class="tex-font-style-bf">multiple times</span> (or not run it at all).</p><p>For example, if the first line of the board looks like that "<span class="tex-font-style-tt">BBBBBBWW</span>" (the white cells of the line are marked with character "<span class="tex-font-style-tt">W</span>", the black cells are marked with character "<span class="tex-font-style-tt">B</span>"), then after one cyclic shift it will look like that "<span class="tex-font-style-tt">WBBBBBBW</span>".</p><p>Help the Little Elephant and his friend to find out whether they can use any number of the described operations to turn the board they have into a proper chessboard.</p></div><div class="input-specification"><p>The input consists of exactly eight lines. Each line contains exactly eight characters "<span class="tex-font-style-tt">W</span>" or "<span class="tex-font-style-tt">B</span>" without any spaces: the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line stands for the color of the <span class="tex-span"><i>j</i></span>-th cell of the <span class="tex-span"><i>i</i></span>-th row of the elephants' board. Character "<span class="tex-font-style-tt">W</span>" stands for the white color, character "<span class="tex-font-style-tt">B</span>" stands for the black color.</p><p>Consider the rows of the board numbered from 1 to 8 from top to bottom, and the columns — from 1 to 8 from left to right. The given board can initially be a proper chessboard.</p></div><div class="output-specification"><p>In a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if we can make the board a proper chessboard and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The input consists of exactly eight lines. Each line contains exactly eight characters "<span class="tex-font-style-tt">W</span>" or "<span class="tex-font-style-tt">B</span>" without any spaces: the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line stands for the color of the <span class="tex-span"><i>j</i></span>-th cell of the <span class="tex-span"><i>i</i></span>-th row of the elephants' board. Character "<span class="tex-font-style-tt">W</span>" stands for the white color, character "<span class="tex-font-style-tt">B</span>" stands for the black color.</p><p>Consider the rows of the board numbered from 1 to 8 from top to bottom, and the columns — from 1 to 8 from left to right. The given board can initially be a proper chessboard.</p>

## Output

<p>In a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if we can make the board a proper chessboard and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
WBWBWBWB
BWBWBWBW
BWBWBWBW
BWBWBWBW
WBWBWBWB
WBWBWBWB
BWBWBWBW
WBWBWBWB

```




```input2
WBWBWBWB
WBWBWBWB
BBWBWWWB
BWBWBWBW
BWBWBWBW
BWBWBWWW
BWBWBWBW
BWBWBWBW

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample you should shift the following lines one position to the right: the 3-rd, the 6-th, the 7-th and the 8-th.</p><p>In the second sample there is no way you can achieve the goal.</p>
