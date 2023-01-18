## Description

<div><p>Andrewid the Android is a galaxy-known detective. Now he does not investigate any case and is eating chocolate out of boredom.</p><p>A bar of chocolate can be presented as an <span class="tex-span"><i>n</i> × <i>n</i></span> table, where each cell represents one piece of chocolate. The columns of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right and the rows are numbered from top to bottom. Let's call the anti-diagonal to be a diagonal that goes the lower left corner to the upper right corner of the table. First Andrewid eats all the pieces lying below the anti-diagonal. Then he performs the following <span class="tex-span"><i>q</i></span> actions with the remaining triangular part: first, he chooses a piece on the anti-diagonal and either direction 'up' or 'left', and then he begins to eat all the pieces starting from the selected cell, moving in the selected direction until he reaches the already eaten piece or chocolate bar edge.</p><p>After each action, he wants to know how many pieces he ate as a result of this action.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the size of the chocolate bar and the number of actions.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the actions: the <span class="tex-span"><i>i</i></span>-th of them contains numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub> = <i>n</i> + 1</span>) — the numbers of the column and row of the chosen cell and the character that represents the direction (<span class="tex-font-style-tt">L</span> — left, <span class="tex-font-style-tt">U</span> — up).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the number of eaten pieces as a result of the <span class="tex-span"><i>i</i></span>-th action.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the size of the chocolate bar and the number of actions.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the actions: the <span class="tex-span"><i>i</i></span>-th of them contains numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub> = <i>n</i> + 1</span>) — the numbers of the column and row of the chosen cell and the character that represents the direction (<span class="tex-font-style-tt">L</span> — left, <span class="tex-font-style-tt">U</span> — up).</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the number of eaten pieces as a result of the <span class="tex-span"><i>i</i></span>-th action.</p>





```input1
6 5
3 4 U
6 1 L
2 5 L
1 6 U
4 3 U

```




```input2
10 6
2 9 U
10 1 U
1 10 U
8 3 L
10 1 L
6 5 U

```




```output1
4
3
2
1
2

```




```output2
9
1
10
6
0
2

```



## Note

<p>Pictures to the sample tests:</p><p><img class="tex-graphics" src="file://ZKfQHx6y.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The pieces that were eaten in the same action are painted the same color. The pieces lying on the anti-diagonal contain the numbers of the action as a result of which these pieces were eaten.</p><p>In the second sample test the Andrewid tries to start eating chocolate for the second time during his fifth action, starting from the cell at the intersection of the 10-th column and the 1-st row, but this cell is already empty, so he does not eat anything.</p>
