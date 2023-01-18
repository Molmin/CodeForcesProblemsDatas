## Description

<div><p>Arthur has bought a beautiful big table into his new flat. When he came home, Arthur noticed that the new table is unstable.</p><p>In total the table Arthur bought has <span class="tex-span"><i>n</i></span> legs, the length of the <span class="tex-span"><i>i</i></span>-th leg is <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Arthur decided to make the table stable and remove some legs. For each of them Arthur determined number <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;—&nbsp;the amount of energy that he spends to remove the <span class="tex-span"><i>i</i></span>-th leg.</p><p>A table with <span class="tex-span"><i>k</i></span> legs is assumed to be stable if there are more than half legs of the maximum length. For example, to make a table with <span class="tex-span">5</span> legs stable, you need to make sure it has at least three (out of these five) legs of the maximum length. Also, a table with one leg is always stable and a table with two legs is stable if and only if they have the same lengths.</p><p>Your task is to help Arthur and count the minimum number of energy units Arthur should spend on making the table stable.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the initial number of legs in the table Arthur bought.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is equal to the length of the <span class="tex-span"><i>i</i></span>-th leg of the table.</p><p>The third line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of energy units that Arthur spends on removing the <span class="tex-span"><i>i</i></span>-th leg off the table.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of energy units that Arthur needs to spend in order to make the table stable.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the initial number of legs in the table Arthur bought.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is equal to the length of the <span class="tex-span"><i>i</i></span>-th leg of the table.</p><p>The third line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of energy units that Arthur spends on removing the <span class="tex-span"><i>i</i></span>-th leg off the table.</p>

## Output

<p>Print a single integer — the minimum number of energy units that Arthur needs to spend in order to make the table stable.</p>





```input1
2
1 5
3 2

```




```input2
3
2 4 4
1 1 1

```




```input3
6
2 2 1 1 3 3
4 3 5 5 2 1

```




```output1
2

```




```output2
0

```




```output3
8

```


