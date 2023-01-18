## Description

<div><p>There is a new TV game on BerTV. In this game two players get a number <span class="tex-span"><i>A</i></span> consisting of <span class="tex-span">2<i>n</i></span> digits. Before each turn players determine who will make the next move. Each player should make exactly <span class="tex-span"><i>n</i></span> moves. On it's turn <span class="tex-span"><i>i</i></span>-th player takes the leftmost digit of <span class="tex-span"><i>A</i></span> and appends it to his or her number <span class="tex-span"><i>S</i><sub class="lower-index"><i>i</i></sub></span>. After that this leftmost digit is erased from <span class="tex-span"><i>A</i></span>. Initially the numbers of both players (<span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span>) are «empty». Leading zeroes in numbers <span class="tex-span"><i>A</i>, <i>S</i><sub class="lower-index">1</sub>, <i>S</i><sub class="lower-index">2</sub></span> are allowed. In the end of the game the first player gets <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span> dollars, and the second gets <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span> dollars.</p><p>One day Homer and Marge came to play the game. They managed to know the number <span class="tex-span"><i>A</i></span> beforehand. They want to find such sequence of their moves that both of them makes exactly <span class="tex-span"><i>n</i></span> moves and which maximizes their total prize. Help them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>). The second line contains integer <span class="tex-span"><i>A</i></span> consisting of exactly <span class="tex-span">2<i>n</i></span> digits. This number can have leading zeroes.</p></div><div class="output-specification"><p>Output the line of <span class="tex-span">2<i>n</i></span> characters <span class="tex-font-style-tt">«H»</span> and <span class="tex-font-style-tt">«M»</span> — the sequence of moves of Homer and Marge, which gives them maximum possible total prize. Each player must make exactly <span class="tex-span"><i>n</i></span> moves. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>). The second line contains integer <span class="tex-span"><i>A</i></span> consisting of exactly <span class="tex-span">2<i>n</i></span> digits. This number can have leading zeroes.</p>

## Output

<p>Output the line of <span class="tex-span">2<i>n</i></span> characters <span class="tex-font-style-tt">«H»</span> and <span class="tex-font-style-tt">«M»</span> — the sequence of moves of Homer and Marge, which gives them maximum possible total prize. Each player must make exactly <span class="tex-span"><i>n</i></span> moves. If there are several solutions, output any of them.</p>





```input1
2
1234

```




```input2
2
9911

```




```output1
HHMM
```




```output2
HMHM
```


