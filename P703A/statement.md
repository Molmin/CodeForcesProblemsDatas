## Description

<div><p>Mishka is a little polar bear. As known, little bears loves spending their free time playing dice for chocolates. Once in a wonderful sunny morning, walking around blocks of ice, Mishka met her friend Chris, and they started playing the game.</p><p>Rules of the game are very simple: at first number of rounds <span class="tex-span"><i>n</i></span> is defined. In every round each of the players throws a cubical dice with distinct numbers from <span class="tex-span">1</span> to <span class="tex-span">6</span> written on its faces. Player, whose value after throwing the dice is greater, wins the round. In case if player dice values are equal, no one of them is a winner.</p><p>In average, player, who won most of the rounds, is the winner of the game. In case if two players won the same number of rounds, the result of the game is draw.</p><p>Mishka is still very little and can't count wins and losses, so she asked you to watch their game and determine its result. Please help her!</p></div><div class="input-specification"><p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of game rounds.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains rounds description. <span class="tex-span"><i>i</i></span>-th of them contains pair of integers <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub>,  <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>)&nbsp;— values on dice upper face after Mishka's and Chris' throws in <span class="tex-span"><i>i</i></span>-th round respectively.</p></div><div class="output-specification"><p>If Mishka is the winner of the game, print <span class="tex-font-style-tt">"Mishka"</span> (without quotes) in the only line.</p><p>If Chris is the winner of the game, print <span class="tex-font-style-tt">"Chris"</span> (without quotes) in the only line.</p><p>If the result of the game is draw, print <span class="tex-font-style-tt">"Friendship is magic!^^"</span> (without quotes) in the only line.</p></div>

## Input

<p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of game rounds.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains rounds description. <span class="tex-span"><i>i</i></span>-th of them contains pair of integers <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub>,  <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>)&nbsp;— values on dice upper face after Mishka's and Chris' throws in <span class="tex-span"><i>i</i></span>-th round respectively.</p>

## Output

<p>If Mishka is the winner of the game, print <span class="tex-font-style-tt">"Mishka"</span> (without quotes) in the only line.</p><p>If Chris is the winner of the game, print <span class="tex-font-style-tt">"Chris"</span> (without quotes) in the only line.</p><p>If the result of the game is draw, print <span class="tex-font-style-tt">"Friendship is magic!^^"</span> (without quotes) in the only line.</p>





```input1
3
3 5
2 1
4 2

```




```input2
2
6 1
1 6

```




```input3
3
1 5
3 3
2 2

```




```output1
Mishka
```




```output2
Friendship is magic!^^
```




```output3
Chris
```



## Note

<p>In the first sample case Mishka loses the first round, but wins second and third rounds and thus she is the winner of the game.</p><p>In the second sample case Mishka wins the first round, Chris wins the second round, and the game ends with draw with score 1:1.</p><p>In the third sample case Chris wins the first round, but there is no winner of the next two rounds. The winner of the game is Chris.</p>
