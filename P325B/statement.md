## Description

<div><p>Daniel is organizing a football tournament. He has come up with the following tournament format: </p><ol> <li> In the first several (possibly zero) stages, while the number of teams is even, they split in pairs and play one game for each pair. At each stage the loser of each pair is eliminated (there are no draws). Such stages are held while the number of teams is even. </li><li> Eventually there will be an odd number of teams remaining. If there is one team remaining, it will be declared the winner, and the tournament ends. Otherwise each of the remaining teams will play with each other remaining team once in round robin tournament (if there are <span class="tex-span"><i>x</i></span> teams, there will be <img align="middle" class="tex-formula" src="file://SubYIHWa.png" style="max-width: 100.0%;max-height: 100.0%;"> games), and the tournament ends. </li></ol><p>For example, if there were 20 teams initially, they would begin by playing 10 games. So, 10 teams would be eliminated, and the remaining 10 would play 5 games. Then the remaining 5 teams would play 10 games in a round robin tournament. In total there would be 10+5+10=25 games.</p><p>Daniel has already booked the stadium for <span class="tex-span"><i>n</i></span> games. Help him to determine how many teams he should invite so that the tournament needs <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>n</i></span> games. You should print all possible numbers of teams that will yield exactly <span class="tex-span"><i>n</i></span> games in ascending order, or <span class="tex-font-style-tt">-1</span> if there are no such numbers.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>), the number of games that should be played.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print all possible numbers of invited teams in ascending order, one per line. If exactly <span class="tex-span"><i>n</i></span> games cannot be played, output one number: <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>), the number of games that should be played.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print all possible numbers of invited teams in ascending order, one per line. If exactly <span class="tex-span"><i>n</i></span> games cannot be played, output one number: <span class="tex-font-style-tt">-1</span>.</p>





```input1
3

```




```input2
25

```




```input3
2

```




```output1
3
4

```




```output2
20

```




```output3
-1

```


