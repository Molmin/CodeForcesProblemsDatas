## Description

<div><p>Physicist Woll likes to play one relaxing game in between his search of the theory of everything.</p><p>Game interface consists of a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span> playing field and a dashboard. Initially some cells of the playing field are filled while others are empty. Dashboard contains images of all various connected (we mean connectivity by side) figures of 2, 3, 4 and 5 cells, with all their rotations and reflections. Player can copy any figure from the dashboard and place it anywhere at the still empty cells of the playing field. Of course any figure can be used as many times as needed.</p><p>Woll's aim is to fill the whole field in such a way that there are no empty cells left, and also... just have some fun.</p><p>Every initially empty cell should be filled with exactly one cell of some figure. Every figure should be entirely inside the board.</p><center> <img class="tex-graphics" src="file://ZjrdDHcG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the picture black cells stand for initially filled cells of the field, and one-colour regions represent the figures.</p></div><div class="input-specification"><p>First line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the height and the width of the field correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each. They represent the field in a natural way: <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is "<span class="tex-font-style-tt">#</span>" if the corresponding cell is filled, and "<span class="tex-font-style-tt">.</span>" if it is empty.</p></div><div class="output-specification"><p>If there is no chance to win the game output the only number "-1" (without the quotes). Otherwise output any filling of the field by the figures in the following format: each figure should be represented by some digit and figures that touch each other by side should be represented by distinct digits. Every initially filled cell should be represented by "<span class="tex-font-style-tt">#</span>".</p></div>

## Input

<p>First line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the height and the width of the field correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each. They represent the field in a natural way: <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line is "<span class="tex-font-style-tt">#</span>" if the corresponding cell is filled, and "<span class="tex-font-style-tt">.</span>" if it is empty.</p>

## Output

<p>If there is no chance to win the game output the only number "-1" (without the quotes). Otherwise output any filling of the field by the figures in the following format: each figure should be represented by some digit and figures that touch each other by side should be represented by distinct digits. Every initially filled cell should be represented by "<span class="tex-font-style-tt">#</span>".</p>





```input1
2 3
...
#.#

```




```input2
3 3
.#.
...
..#

```




```input3
3 3
...
.##
.#.

```




```input4
1 2
##

```




```output1
000
#0#

```




```output2
5#1
511
55#

```




```output3
-1

```




```output4
##

```



## Note

<p>In the third sample, there is no way to fill a cell with no empty neighbours.</p><p>In the forth sample, Woll does not have to fill anything, so we should output the field from the input.</p>
