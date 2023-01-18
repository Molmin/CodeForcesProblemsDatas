## Description

<div><p>Bishwock is a chess figure that consists of three squares resembling an "L-bar". This figure can be rotated by 90, 180 and 270 degrees so it can have four possible states:</p><center> <pre class="verbatim"><br>XX   XX   .X   X.<br>X.   .X   XX   XX<br></pre> </center><p>Bishwocks don't attack any squares and can even occupy on the adjacent squares as long as they don't occupy the same square. </p><p>Vasya has a board with $2\times n$ squares onto which he wants to put some bishwocks. To his dismay, several squares on this board are already occupied by pawns and Vasya can't put bishwocks there. However, pawns also don't attack bishwocks and they can occupy adjacent squares peacefully.</p><p>Knowing the positions of pawns on the board, help Vasya to determine the maximum amount of bishwocks he can put onto the board so that they wouldn't occupy the same squares and wouldn't occupy squares with pawns.</p></div><div class="input-specification"><p>The input contains two nonempty strings that describe Vasya's board. Those strings contain only symbols "<span class="tex-font-style-tt">0</span>" (zero) that denote the empty squares and symbols "<span class="tex-font-style-tt">X</span>" (uppercase English letter) that denote the squares occupied by pawns. Strings are nonempty and are of the same length that does not exceed $100$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the maximum amount of bishwocks that can be placed onto the given board.</p></div>

## Input

<p>The input contains two nonempty strings that describe Vasya's board. Those strings contain only symbols "<span class="tex-font-style-tt">0</span>" (zero) that denote the empty squares and symbols "<span class="tex-font-style-tt">X</span>" (uppercase English letter) that denote the squares occupied by pawns. Strings are nonempty and are of the same length that does not exceed $100$.</p>

## Output

<p>Output a single integer&nbsp;— the maximum amount of bishwocks that can be placed onto the given board.</p>





```input1
00
00

```




```input2
00X00X0XXX0
0XXX0X00X00

```




```input3
0X0X0
0X0X0

```




```input4
0XXX0
00000

```




```output1
1
```




```output2
4
```




```output3
0
```




```output4
2
```


