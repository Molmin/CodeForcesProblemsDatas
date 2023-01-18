## Description

<div><p>Hooray! Berl II, the king of Berland is making a knight tournament. The king has already sent the message to all knights in the kingdom and they in turn agreed to participate in this grand event.</p><p>As for you, you're just a simple peasant. There's no surprise that you slept in this morning and were late for the tournament (it was a weekend, after all). Now you are really curious about the results of the tournament. This time the tournament in Berland went as follows:</p><ul> <li> There are <span class="tex-span"><i>n</i></span> knights participating in the tournament. Each knight was assigned his unique number — an integer from 1 to <span class="tex-span"><i>n</i></span>. </li><li> The tournament consisted of <span class="tex-span"><i>m</i></span> fights, in the <span class="tex-span"><i>i</i></span>-th fight the knights that were still in the game with numbers at least <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and at most <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> have fought for the right to continue taking part in the tournament. </li><li> After the <span class="tex-span"><i>i</i></span>-th fight among all participants of the fight only one knight won — the knight number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, he continued participating in the tournament. Other knights left the tournament. </li><li> The winner of the last (the <span class="tex-span"><i>m</i></span>-th) fight (the knight number <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i></sub></span>) became the winner of the tournament. </li></ul><p>You fished out all the information about the fights from your friends. Now for each knight you want to know the name of the knight he was conquered by. We think that the knight number <span class="tex-span"><i>b</i></span> was conquered by the knight number <span class="tex-span"><i>a</i></span>, if there was a fight with both of these knights present and the winner was the knight number <span class="tex-span"><i>a</i></span>.</p><p>Write the code that calculates for each knight, the name of the knight that beat him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of knights and the number of fights. Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th fight.</p><p>It is guaranteed that the input is correct and matches the problem statement. It is guaranteed that at least two knights took part in each battle.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers. If the <span class="tex-span"><i>i</i></span>-th knight lost, then the <span class="tex-span"><i>i</i></span>-th number should equal the number of the knight that beat the knight number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th knight is the winner, then the <span class="tex-span"><i>i</i></span>-th number must equal <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of knights and the number of fights. Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th fight.</p><p>It is guaranteed that the input is correct and matches the problem statement. It is guaranteed that at least two knights took part in each battle.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers. If the <span class="tex-span"><i>i</i></span>-th knight lost, then the <span class="tex-span"><i>i</i></span>-th number should equal the number of the knight that beat the knight number <span class="tex-span"><i>i</i></span>. If the <span class="tex-span"><i>i</i></span>-th knight is the winner, then the <span class="tex-span"><i>i</i></span>-th number must equal <span class="tex-span">0</span>.</p>





```input1
4 3
1 2 1
1 3 3
1 4 4

```




```input2
8 4
3 5 4
3 7 6
2 8 8
1 8 1

```




```output1
3 1 4 0
```




```output2
0 8 4 6 4 8 6 1
```



## Note

<p>Consider the first test case. Knights 1 and 2 fought the first fight and knight 1 won. Knights 1 and 3 fought the second fight and knight 3 won. The last fight was between knights 3 and 4, knight 4 won.</p>
