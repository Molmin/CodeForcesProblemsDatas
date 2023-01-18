## Description

<div><p>"Contestant who earns a score equal to or greater than the <span class="tex-span"><i>k</i></span>-th place finisher's score will advance to the next round, as long as the contestant earns a positive score..." — an excerpt from contest rules.</p><p>A total of <span class="tex-span"><i>n</i></span> participants took part in the contest (<span class="tex-span"><i>n</i> ≥ <i>k</i></span>), and you already know their scores. Calculate how many participants will advance to the next round.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>) separated by a single space.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the score earned by the participant who got the <span class="tex-span"><i>i</i></span>-th place. The given sequence is non-increasing (that is, for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> the following condition is fulfilled: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p></div><div class="output-specification"><p>Output the number of participants who advance to the next round.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>) separated by a single space.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the score earned by the participant who got the <span class="tex-span"><i>i</i></span>-th place. The given sequence is non-increasing (that is, for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> the following condition is fulfilled: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p>

## Output

<p>Output the number of participants who advance to the next round.</p>





```input1
8 5
10 9 8 7 7 7 5 5

```




```input2
4 2
0 0 0 0

```




```output1
6

```




```output2
0

```



## Note

<p>In the first example the participant on the 5th place earned 7 points. As the participant on the 6th place also earned 7 points, there are 6 advancers.</p><p>In the second example nobody got a positive score.</p>
