## Description

<div><p>The Smart Beaver from ABBYY decided to have a day off. But doing nothing the whole day turned out to be too boring, and he decided to play a game with pebbles. Initially, the Beaver has <span class="tex-span"><i>n</i></span> pebbles. He arranges them in <span class="tex-span"><i>a</i></span> equal rows, each row has <span class="tex-span"><i>b</i></span> pebbles (<span class="tex-span"><i>a</i> &gt; 1</span>). Note that the Beaver must use all the pebbles he has, i. e. <span class="tex-span"><i>n</i> = <i>a</i>·<i>b</i></span>.</p><center> <img class="tex-graphics" src="file://beLesF34.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> 10 pebbles are arranged in two rows, each row has 5 pebbles </span> </center><p>Once the Smart Beaver has arranged the pebbles, he takes back any of the resulting rows (that is, <span class="tex-span"><i>b</i></span> pebbles) and discards all other pebbles. Then he arranges <span class="tex-font-style-bf">all</span> his pebbles again (possibly choosing other values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>) and takes back one row, and so on. The game continues until at some point the Beaver ends up with exactly one pebble. </p><p>The game process can be represented as a finite sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span>, where: </p><ul> <li> <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> = <i>n</i></span> </li><li> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> is the number of pebbles that the Beaver ends up with after the <span class="tex-span"><i>i</i></span>-th move, that is, the number of pebbles in a row after some arrangement of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> pebbles (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>). Note that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> &gt; <i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </li><li> <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub> = 1</span> </li></ul><p>The result of the game is the sum of numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. You are given <span class="tex-span"><i>n</i></span>. Find the maximum possible result of the game.</p></div><div class="input-specification"><p>The single line of the input contains a single integer <span class="tex-span"><i>n</i></span> — the initial number of pebbles the Smart Beaver has.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i> ≤ 50</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span> </li></ul> </div><div class="output-specification"><p>Print a single number — the maximum possible result of the game.</p></div>

## Input

<p>The single line of the input contains a single integer <span class="tex-span"><i>n</i></span> — the initial number of pebbles the Smart Beaver has.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i> ≤ 50</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span> </li></ul>

## Output

<p>Print a single number — the maximum possible result of the game.</p>





```input1
10

```




```input2
8

```




```output1
16

```




```output2
15

```



## Note

<p>Consider the first example (<span class="tex-span"><i>c</i><sub class="lower-index">1</sub> = 10</span>). The possible options for the game development are:</p><ul> <li> Arrange the pebbles in 10 rows, one pebble per row. Then <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = 1</span>, and the game ends after the first move with the result of 11. </li><li> Arrange the pebbles in 5 rows, two pebbles per row. Then <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = 2</span>, and the game continues. During the second move we have two pebbles which can be arranged in a unique way (remember that you are not allowed to put all the pebbles in the same row!) — 2 rows, one pebble per row. <span class="tex-span"><i>c</i><sub class="lower-index">3</sub> = 1</span>, and the game ends with the result of 13. </li><li> Finally, arrange the pebbles in two rows, five pebbles per row. The same logic leads us to <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = 5, <i>c</i><sub class="lower-index">3</sub> = 1</span>, and the game ends with the result of 16 — the maximum possible result. </li></ul>
