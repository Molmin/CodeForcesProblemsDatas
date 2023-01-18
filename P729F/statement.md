## Description

<div><p><span class="tex-font-style-it">This problem has unusual memory constraint.</span></p><p>At evening, Igor and Zhenya the financiers became boring, so they decided to play a game. They prepared <span class="tex-span"><i>n</i></span> papers with the income of some company for some time periods. Note that the income can be positive, zero or negative.</p><p>Igor and Zhenya placed the papers in a row and decided to take turns making moves. Igor will take the papers from the left side, Zhenya will take the papers from the right side. Igor goes first and takes <span class="tex-span">1</span> or <span class="tex-span">2</span> (on his choice) papers from the left. Then, on each turn a player can take <span class="tex-span"><i>k</i></span> or <span class="tex-span"><i>k</i> + 1</span> papers from his side if the opponent took exactly <span class="tex-span"><i>k</i></span> papers in the previous turn. Players can't skip moves. The game ends when there are no papers left, or when some of the players can't make a move.</p><p>Your task is to determine the difference between the sum of incomes on the papers Igor took and the sum of incomes on the papers Zhenya took, assuming both players play optimally. Igor wants to maximize the difference, Zhenya wants to minimize it.</p></div><div class="input-specification"><p>The first line contains single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>)&nbsp;— the number of papers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the income on the <span class="tex-span"><i>i</i></span>-th paper from the left.</p></div><div class="output-specification"><p>Print the difference between the sum of incomes on the papers Igor took and the sum of incomes on the papers Zhenya took, assuming both players play optimally. Igor wants to maximize the difference, Zhenya wants to minimize it.</p></div>

## Input

<p>The first line contains single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>)&nbsp;— the number of papers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the income on the <span class="tex-span"><i>i</i></span>-th paper from the left.</p>

## Output

<p>Print the difference between the sum of incomes on the papers Igor took and the sum of incomes on the papers Zhenya took, assuming both players play optimally. Igor wants to maximize the difference, Zhenya wants to minimize it.</p>





```input1
3
1 3 1

```




```input2
5
-1 -2 -1 -2 -1

```




```input3
4
-4 -2 4 5

```




```output1
4

```




```output2
0

```




```output3
-13

```



## Note

<p>In the first example it's profitable for Igor to take two papers from the left to have the sum of the incomes equal to <span class="tex-span">4</span>. Then Zhenya wouldn't be able to make a move since there would be only one paper, and he would be able to take only <span class="tex-span">2</span> or <span class="tex-span">3</span>..</p>
