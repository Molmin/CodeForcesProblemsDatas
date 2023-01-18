## Description

<div><p>Petya and Vasya decided to play a game. They have <span class="tex-span"><i>n</i></span> cards (<span class="tex-span"><i>n</i></span> is an even number). A single integer is written on each card.</p><p>Before the game Petya will choose an integer and after that Vasya will choose another integer (<span class="tex-font-style-bf">different</span> from the number that Petya chose). During the game each player takes all the cards with number he chose. For example, if Petya chose number <span class="tex-span">5</span> before the game he will take all cards on which <span class="tex-span">5</span> is written and if Vasya chose number <span class="tex-span">10</span> before the game he will take all cards on which <span class="tex-span">10</span> is written.</p><p>The game is considered fair if Petya and Vasya can take all <span class="tex-span"><i>n</i></span> cards, and the number of cards each player gets is the same.</p><p>Determine whether Petya and Vasya can choose integer numbers before the game so that the game is fair. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — number of cards. It is guaranteed that <span class="tex-span"><i>n</i></span> is an even number.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (one integer per line, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — numbers written on the <span class="tex-span"><i>n</i></span> cards.</p></div><div class="output-specification"><p>If it is impossible for Petya and Vasya to choose numbers in such a way that the game will be fair, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line. In this case you should not print anything more.</p><p>In the other case print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print two distinct integers — number that Petya should choose and the number that Vasya should choose to make the game fair. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — number of cards. It is guaranteed that <span class="tex-span"><i>n</i></span> is an even number.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (one integer per line, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — numbers written on the <span class="tex-span"><i>n</i></span> cards.</p>

## Output

<p>If it is impossible for Petya and Vasya to choose numbers in such a way that the game will be fair, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line. In this case you should not print anything more.</p><p>In the other case print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print two distinct integers — number that Petya should choose and the number that Vasya should choose to make the game fair. If there are several solutions, print any of them.</p>





```input1
4
11
27
27
11

```




```input2
2
6
6

```




```input3
6
10
20
30
20
10
20

```




```input4
6
1
1
2
2
3
3

```




```output1
YES
11 27

```




```output2
NO

```




```output3
NO

```




```output4
NO

```



## Note

<p>In the first example the game will be fair if, for example, Petya chooses number <span class="tex-span">11</span>, and Vasya chooses number <span class="tex-span">27</span>. Then the will take all cards — Petya will take cards <span class="tex-span">1</span> and <span class="tex-span">4</span>, and Vasya will take cards <span class="tex-span">2</span> and <span class="tex-span">3</span>. Thus, each of them will take exactly two cards.</p><p>In the second example fair game is impossible because the numbers written on the cards are equal, but the numbers that Petya and Vasya should choose should be distinct.</p><p>In the third example it is impossible to take all cards. Petya and Vasya can take at most five cards — for example, Petya can choose number <span class="tex-span">10</span> and Vasya can choose number <span class="tex-span">20</span>. But for the game to be fair it is necessary to take <span class="tex-span">6</span> cards.</p>
