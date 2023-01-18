## Description

<div><p>Ivan has <span class="tex-span"><i>n</i></span> different boxes. The first of them contains some balls of <span class="tex-span"><i>n</i></span> different colors.</p><p>Ivan wants to play a strange game. He wants to distribute the balls into boxes in such a way that for every <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) <span class="tex-span"><i>i</i></span>-th box will contain all balls with color <span class="tex-span"><i>i</i></span>.</p><p>In order to do this, Ivan will make some turns. Each turn he does the following:</p><ol> <li> Ivan chooses any non-empty box and takes all balls from this box; </li><li> Then Ivan chooses any <span class="tex-span"><i>k</i></span> empty boxes (the box from the first step becomes empty, and Ivan is allowed to choose it), separates the balls he took on the previous step into <span class="tex-span"><i>k</i></span> non-empty groups and puts each group into one of the boxes. He should put each group into a separate box. He can choose either <span class="tex-span"><i>k</i> = 2</span> or <span class="tex-span"><i>k</i> = 3</span>. </li></ol><p>The <span class="tex-font-style-it">penalty</span> of the turn is the number of balls Ivan takes from the box during the first step of the turn. And <span class="tex-font-style-it">penalty</span> of the game is the total <span class="tex-font-style-it">penalty</span> of turns made by Ivan until he distributes all balls to corresponding boxes.</p><p>Help Ivan to determine the minimum possible <span class="tex-font-style-it">penalty</span> of the game!</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of boxes and colors.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of balls with color <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print one number — the minimum possible <span class="tex-font-style-it">penalty</span> of the game.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of boxes and colors.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of balls with color <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print one number — the minimum possible <span class="tex-font-style-it">penalty</span> of the game.</p>





```input1
3
1 2 3

```




```input2
4
2 3 4 5

```




```output1
6

```




```output2
19

```



## Note

<p>In the first example you take all the balls from the first box, choose <span class="tex-span"><i>k</i> = 3</span> and sort all colors to corresponding boxes. Penalty is <span class="tex-span">6</span>.</p><p>In the second example you make two turns: </p><ol> <li> Take all the balls from the first box, choose <span class="tex-span"><i>k</i> = 3</span>, put balls of color <span class="tex-span">3</span> to the third box, of color <span class="tex-span">4</span> — to the fourth box and the rest put back into the first box. Penalty is <span class="tex-span">14</span>; </li><li> Take all the balls from the first box, choose <span class="tex-span"><i>k</i> = 2</span>, put balls of color <span class="tex-span">1</span> to the first box, of color <span class="tex-span">2</span> — to the second box. Penalty is <span class="tex-span">5</span>. </li></ol><p>Total penalty is <span class="tex-span">19</span>.</p>
