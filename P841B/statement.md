## Description

<div><p>Leha somehow found an array consisting of <span class="tex-span"><i>n</i></span> integers. Looking at it, he came up with a task. Two players play the game on the array. Players move one by one. The first player can choose for his move a subsegment of non-zero length with an odd sum of numbers and remove it from the array, after that the remaining parts are glued together into one array and the game continues. The second player can choose a subsegment of non-zero length with an even sum and remove it. Loses the one who can not make a move. Who will win if both play optimally?</p></div><div class="input-specification"><p>First line of input data contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output answer in single line. "<span class="tex-font-style-tt">First</span>", if first player wins, and "<span class="tex-font-style-tt">Second</span>" otherwise (without quotes).</p></div>

## Input

<p>First line of input data contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output answer in single line. "<span class="tex-font-style-tt">First</span>", if first player wins, and "<span class="tex-font-style-tt">Second</span>" otherwise (without quotes).</p>





```input1
4
1 3 2 3

```




```input2
2
2 2

```




```output1
First

```




```output2
Second

```



## Note

<p>In first sample first player remove whole array in one move and win.</p><p>In second sample first player can't make a move and lose.</p>
