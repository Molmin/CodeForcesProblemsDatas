## Description

<div><p><span class="tex-span"><i>n</i></span> people are standing in a line to play table tennis. At first, the first two players in the line play a game. Then the loser goes to the end of the line, and the winner plays with the next person from the line, and so on. They play until someone wins <span class="tex-span"><i>k</i></span> games in a row. This player becomes the winner.</p><p>For each of the participants, you know the power to play table tennis, and for all players these values are different. In a game the player with greater power always wins. Determine who will be the winner.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>)&nbsp;— the number of people and the number of wins.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — powers of the player. It's guaranteed that this line contains a valid permutation, i.e. all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Output a single integer — <span class="tex-font-style-bf">power</span> of the winner.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>)&nbsp;— the number of people and the number of wins.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — powers of the player. It's guaranteed that this line contains a valid permutation, i.e. all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Output a single integer — <span class="tex-font-style-bf">power</span> of the winner.</p>





```input1
2 2
1 2

```




```input2
4 2
3 1 2 4

```




```input3
6 2
6 5 3 1 2 4

```




```input4
2 10000000000
2 1

```




```output1
2
```




```output2
3
```




```output3
6
```




```output4
2

```



## Note

<p>Games in the second sample:</p><p><span class="tex-span">3</span> plays with <span class="tex-span">1</span>. <span class="tex-span">3</span> wins. <span class="tex-span">1</span> goes to the end of the line.</p><p><span class="tex-span">3</span> plays with <span class="tex-span">2</span>. <span class="tex-span">3</span> wins. He wins twice in a row. He becomes the winner.</p>
