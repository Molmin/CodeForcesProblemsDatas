## Description

<div><p>The tournament «Sleepyhead-2010» in the rapid falling asleep has just finished in Berland. <span class="tex-span"><i>n</i></span> best participants from the country have participated in it. The tournament consists of games, each of them is a match between two participants. <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> games were played during the tournament, and each participant had a match with each other participant. </p><p>The rules of the game are quite simple — the participant who falls asleep first wins. The secretary made a record of each game in the form «<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>», where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of participants. The first number in each pair is a winner (i.e. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a winner and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is a loser). There is no draws.</p><p>Recently researches form the «Institute Of Sleep» have found that every person is characterized by a value <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> — the speed of falling asleep. The person who has lower speed wins. Every person has its own value <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>, constant during the life. </p><p>It is known that all participants of the tournament have distinct speeds of falling asleep. Also it was found that the secretary made records about all the games except one. You are to find the result of the missing game.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>) — the number of participants. The following <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2 - 1</span> lines contain the results of the games. Each game is described in a single line by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> и <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the opponents in this game. It is known that during the tournament each of the <span class="tex-span"><i>n</i></span> participants played <span class="tex-span"><i>n</i> - 1</span> games, one game with each other participant.</p></div><div class="output-specification"><p>Output two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the missing record. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>) — the number of participants. The following <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2 - 1</span> lines contain the results of the games. Each game is described in a single line by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> и <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the opponents in this game. It is known that during the tournament each of the <span class="tex-span"><i>n</i></span> participants played <span class="tex-span"><i>n</i> - 1</span> games, one game with each other participant.</p>

## Output

<p>Output two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the missing record. If there are several solutions, output any of them.</p>





```input1
4
4 2
4 1
2 3
2 1
3 1

```




```output1
4 3

```


