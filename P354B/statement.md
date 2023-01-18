## Description

<div><p>Given an <span class="tex-span"><i>n</i> × <i>n</i></span> table <span class="tex-span"><i>T</i></span> consisting of lowercase English letters. We'll consider some string <span class="tex-span"><i>s</i></span> <span class="tex-font-style-it">good</span> if the table contains a correct path corresponding to the given string. In other words, good strings are all strings we can obtain by moving from the left upper cell of the table only to the right and down. Here's the formal definition of correct paths:</p><p>Consider rows of the table are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and columns of the table are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to the right. Cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> is a cell of table <span class="tex-span"><i>T</i></span> on the <span class="tex-span"><i>r</i></span>-th row and in the <span class="tex-span"><i>c</i></span>-th column. This cell corresponds to letter <span class="tex-span"><i>T</i><sub class="lower-index"><i>r</i>, <i>c</i></sub></span>.</p><p>A path of length <span class="tex-span"><i>k</i></span> is a sequence of table cells <span class="tex-span">[(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>), (<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>), ..., (<i>r</i><sub class="lower-index"><i>k</i></sub>, <i>c</i><sub class="lower-index"><i>k</i></sub>)]</span>. The following paths are correct: </p><ol> <li> There is only one correct path of length <span class="tex-span">1</span>, that is, consisting of a single cell: <span class="tex-span">[(1, 1)]</span>; </li><li> Let's assume that <span class="tex-span">[(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>), ..., (<i>r</i><sub class="lower-index"><i>m</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub>)]</span> is a correct path of length <span class="tex-span"><i>m</i></span>, then paths <span class="tex-span">[(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>), ..., (<i>r</i><sub class="lower-index"><i>m</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub>), (<i>r</i><sub class="lower-index"><i>m</i></sub> + 1, <i>c</i><sub class="lower-index"><i>m</i></sub>)]</span> and <span class="tex-span">[(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>), ..., (<i>r</i><sub class="lower-index"><i>m</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub>), (<i>r</i><sub class="lower-index"><i>m</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub> + 1)]</span> are correct paths of length <span class="tex-span"><i>m</i> + 1</span>. </li></ol><p>We should assume that a path <span class="tex-span">[(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>), (<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>), ..., (<i>r</i><sub class="lower-index"><i>k</i></sub>, <i>c</i><sub class="lower-index"><i>k</i></sub>)]</span> corresponds to a string of length <span class="tex-span"><i>k</i></span>: <span class="tex-span"><i>T</i><sub class="lower-index"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub></sub> + <i>T</i><sub class="lower-index"><i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></sub> + ... + <i>T</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>k</i></sub>, <i>c</i><sub class="lower-index"><i>k</i></sub></sub></span>.</p><p>Two players play the following game: initially they have an empty string. Then the players take turns to add a letter to the end of the string. After each move (adding a new letter) the resulting string must be good. The game ends after <span class="tex-span">2<i>n</i> - 1</span> turns. A player wins by the following scenario: </p><ol> <li> If the resulting string has strictly more letters "<span class="tex-font-style-tt">a</span>" than letters "<span class="tex-font-style-tt">b</span>", then the first player wins; </li><li> If the resulting string has strictly more letters "<span class="tex-font-style-tt">b</span>" than letters "<span class="tex-font-style-tt">a</span>", then the second player wins; </li><li> If the resulting string has the same number of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>", then the players end the game with a draw. </li></ol><p>Your task is to determine the result of the game provided that both players played optimally well.</p></div><div class="input-specification"><p>The first line contains a single number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> lowercase English letters each — table <span class="tex-span"><i>T</i></span>.</p></div><div class="output-specification"><p>In a single line print string "<span class="tex-font-style-tt">FIRST</span>", if the first player wins, "<span class="tex-font-style-tt">SECOND</span>", if the second player wins and "<span class="tex-font-style-tt">DRAW</span>", if the game ends with a draw.</p></div>

## Input

<p>The first line contains a single number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> lowercase English letters each — table <span class="tex-span"><i>T</i></span>.</p>

## Output

<p>In a single line print string "<span class="tex-font-style-tt">FIRST</span>", if the first player wins, "<span class="tex-font-style-tt">SECOND</span>", if the second player wins and "<span class="tex-font-style-tt">DRAW</span>", if the game ends with a draw.</p>





```input1
2
ab
cd

```




```input2
2
xa
ay

```




```input3
3
aab
bcb
bac

```




```output1
DRAW

```




```output2
FIRST

```




```output3
DRAW

```



## Note

<p>Consider the first sample:</p><p>Good strings are strings: <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">ac</span>, <span class="tex-font-style-tt">abd</span>, <span class="tex-font-style-tt">acd</span>.</p><p>The first player moves first and adds letter <span class="tex-font-style-tt">a</span> to the string, as there is only one good string of length <span class="tex-span">1</span>. Then the second player can add <span class="tex-font-style-tt">b</span> or <span class="tex-font-style-tt">c</span> and the game will end with strings <span class="tex-font-style-tt">abd</span> or <span class="tex-font-style-tt">acd</span>, correspondingly. In the first case it will be a draw (the string has one <span class="tex-font-style-tt">a</span> and one <span class="tex-font-style-tt">b</span>), in the second case the first player wins. Naturally, in this case the second player prefers to choose letter <span class="tex-font-style-tt">b</span> and end the game with a draw.</p><p>Consider the second sample:</p><p>Good strings are: <span class="tex-font-style-tt">x</span>, <span class="tex-font-style-tt">xa</span>, <span class="tex-font-style-tt">xay</span>.</p><p>We can see that the game will end with string <span class="tex-font-style-tt">xay</span> and the first player wins.</p>
