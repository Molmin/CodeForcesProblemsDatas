## Description

<div><p>One university has just found out about a sport programming contest called ACM ICPC v2.0. This contest doesn't differ much from the well-known ACM ICPC, for example, the participants are not allowed to take part in the finals more than two times. However, there is one notable difference: the teams in the contest should consist of exactly <span class="tex-span"><i>n</i></span> participants.</p><p>Having taken part in several ACM ICPC v2.0 finals and having not won any medals, the students and the university governors realized that it's high time they changed something about the preparation process. Specifically, as the first innovation it was decided to change the teams' formation process. Having spent considerable amount of time on studying the statistics of other universities' performance, they managed to receive some interesting information: the dependence between the probability of winning a medal and the number of team members that participated in the finals in the past. More formally, we know <span class="tex-span"><i>n</i> + 1</span> real numbers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub> ≤ <i>p</i><sub class="lower-index">1</sub> ≤ ... ≤ <i>p</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the probability of getting a medal on the finals if the team has <span class="tex-span"><i>i</i></span> participants of previous finals, and other <span class="tex-span"><i>n</i> - <i>i</i></span> participants arrived to the finals for the first time.</p><p>Despite such useful data, the university governors are unable to determine such team forming tactics that would provide the maximum probability of winning a medal at ACM ICPC v2.0 finals on average (we are supposed to want to provide such result to the far future and we are also supposed to have an endless supply of students). And how about you, can you offer such optimal tactic? At the first stage the university governors want to know the value of maximum average probability.</p><p>More formally, suppose that the university sends a team to the <span class="tex-span"><i>k</i></span>-th world finals. The team has <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> participants of previous finals (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). Since each person can participate in the finals no more than twice, the following condition must be true: <img align="middle" class="tex-formula" src="file://oSZZsleD.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to choose sequence <img align="middle" class="tex-formula" src="file://tZDAVuzx.png" style="max-width: 100.0%;max-height: 100.0%;"> so that the limit <span class="tex-span">Ψ</span> exists and it's value is maximal:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://C0QxEfwF.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>As <img align="middle" class="tex-formula" src="file://FjJT88v4.png" style="max-width: 100.0%;max-height: 100.0%;"> is an infinite sequence, you should only print the maximum value of the <span class="tex-span">Ψ</span> limit.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>), <span class="tex-span"><i>n</i></span> is the number of team participants. The second line contains <span class="tex-span"><i>n</i> + 1</span> real numbers with no more than 6 digits after decimal point <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i>, 0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the probability of that the team will win a medal if it contains <span class="tex-span"><i>i</i></span> participants who has already been on the finals. Also the condition <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> should be fulfilled for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i> - 1</span>.</p></div><div class="output-specification"><p>Print the only real number — the expected average number of medals won per year if the optimal strategy is used. The result may have absolute or relative error <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>), <span class="tex-span"><i>n</i></span> is the number of team participants. The second line contains <span class="tex-span"><i>n</i> + 1</span> real numbers with no more than 6 digits after decimal point <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i>, 0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the probability of that the team will win a medal if it contains <span class="tex-span"><i>i</i></span> participants who has already been on the finals. Also the condition <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> should be fulfilled for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i> - 1</span>.</p>

## Output

<p>Print the only real number — the expected average number of medals won per year if the optimal strategy is used. The result may have absolute or relative error <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
0.115590 0.384031 0.443128 0.562356

```




```input2
3
1 1 1 1

```




```output1
0.4286122500

```




```output2
0.9999999999

```



## Note

<p>In the second test, no matter what participants the team contains, it is doomed to be successful.</p>
