## Description

<div><p>Limak is an old brown bear. He often goes bowling with his friends. Today he feels really good and tries to beat his own record!</p><p>For rolling a ball one gets a score — an integer (maybe negative) number of points. Score for the <span class="tex-span"><i>i</i></span>-th roll is multiplied by <span class="tex-span"><i>i</i></span> and scores are summed up. So, for <span class="tex-span"><i>k</i></span> rolls with scores <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, the total score is <img align="middle" class="tex-formula" src="file://xhuSW0T8.png" style="max-width: 100.0%;max-height: 100.0%;">. The total score is <span class="tex-span">0</span> if there were no rolls.</p><p>Limak made <span class="tex-span"><i>n</i></span> rolls and got score <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>-th of them. He wants to maximize his total score and he came up with an interesting idea. He can say that some first rolls were only a warm-up, and that he wasn't focused during the last rolls. More formally, he can cancel any prefix and any suffix of the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. It is allowed to cancel all rolls, or to cancel none of them.</p><p>The total score is calculated as if there were only non-canceled rolls. So, the first non-canceled roll has score multiplied by <span class="tex-span">1</span>, the second one has score multiplied by <span class="tex-span">2</span>, and so on, till the last non-canceled roll.</p><p>What maximum total score can Limak get?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the total number of rolls made by Limak.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> — scores for Limak's rolls.</p></div><div class="output-specification"><p>Print the maximum possible total score after cancelling rolls.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the total number of rolls made by Limak.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> — scores for Limak's rolls.</p>

## Output

<p>Print the maximum possible total score after cancelling rolls.</p>





```input1
6
5 -1000 1 -3 7 -8

```




```input2
5
1000 1000 1001 1000 1000

```




```input3
3
-60 -70 -80

```




```output1
16

```




```output2
15003

```




```output3
0

```



## Note

<p>In the first sample test, Limak should cancel the first two rolls, and one last roll. He will be left with rolls <span class="tex-span">1,  - 3, 7</span> what gives him the total score <span class="tex-span">1·1 + 2·( - 3) + 3·7 = 1 - 6 + 21 = 16</span>.</p>
