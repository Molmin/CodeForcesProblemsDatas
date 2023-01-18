## Description

<div><p>Couple Cover, a wildly popular luck-based game, is about to begin! Two players must work together to construct a rectangle. A bag with <span class="tex-span"><i>n</i></span> balls, each with an integer written on it, is placed on the table. The first player reaches in and grabs a ball randomly (all balls have equal probability of being chosen) — the number written on this ball is the rectangle's width in meters. This ball is not returned to the bag, and the second player reaches into the bag and grabs another ball — the number written on this ball is the rectangle's height in meters. If the area of the rectangle is greater than or equal some threshold <span class="tex-span"><i>p</i></span> square meters, the players win. Otherwise, they lose.</p><p>The organizers of the game are trying to select an appropriate value for <span class="tex-span"><i>p</i></span> so that the probability of a couple winning is not too high and not too low, but they are slow at counting, so they have hired you to answer some questions for them. You are given a list of the numbers written on the balls, the organizers would like to know how many winning pairs of balls exist for different values of <span class="tex-span"><i>p</i></span>. Note that two pairs are different if either the first or the second ball is different between the two in pair, and two different balls with the same number are considered different.</p></div><div class="input-specification"><p>The input begins with a single positive integer <span class="tex-span"><i>n</i></span> in its own line (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers — the <span class="tex-span"><i>i</i></span>-th number in this line is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">6</sup></span>), the number written on the <span class="tex-span"><i>i</i></span>-th ball.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of questions you are being asked.</p><p>Then, the following line contains <span class="tex-span"><i>m</i></span> positive integers — the <span class="tex-span"><i>j</i></span>-th number in this line is equal to the value of <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 3·10<sup class="upper-index">6</sup></span>) in the <span class="tex-span"><i>j</i></span>-th question you are being asked.</p></div><div class="output-specification"><p>For each question, print the number of winning pairs of balls that exist for the given value of <span class="tex-span"><i>p</i></span> in the separate line.</p></div>

## Input

<p>The input begins with a single positive integer <span class="tex-span"><i>n</i></span> in its own line (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers — the <span class="tex-span"><i>i</i></span>-th number in this line is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">6</sup></span>), the number written on the <span class="tex-span"><i>i</i></span>-th ball.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of questions you are being asked.</p><p>Then, the following line contains <span class="tex-span"><i>m</i></span> positive integers — the <span class="tex-span"><i>j</i></span>-th number in this line is equal to the value of <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 3·10<sup class="upper-index">6</sup></span>) in the <span class="tex-span"><i>j</i></span>-th question you are being asked.</p>

## Output

<p>For each question, print the number of winning pairs of balls that exist for the given value of <span class="tex-span"><i>p</i></span> in the separate line.</p>





```input1
5
4 2 6 1 3
4
1 3 5 8

```




```input2
2
5 6
2
30 31

```




```output1
20
18
14
10

```




```output2
2
0

```


