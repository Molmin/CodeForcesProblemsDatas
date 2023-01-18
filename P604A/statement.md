## Description

<div><p>Kevin Sun has just finished competing in Codeforces Round #334! The round was 120 minutes long and featured five problems with maximum point values of 500, 1000, 1500, 2000, and 2500, respectively. Despite the challenging tasks, Kevin was uncowed and bulldozed through all of them, distinguishing himself from the herd as the best cowmputer scientist in all of Bovinia. Kevin knows his submission time for each problem, the number of wrong submissions that he made on each problem, and his total numbers of successful and unsuccessful hacks. Because Codeforces scoring is complicated, Kevin wants you to write a program to compute his final score.</p><p>Codeforces scores are computed as follows: If the maximum point value of a problem is <span class="tex-span"><i>x</i></span>, and Kevin submitted correctly at minute <span class="tex-span"><i>m</i></span> but made <span class="tex-span"><i>w</i></span> wrong submissions, then his score on that problem is <img align="middle" class="tex-formula" src="file://y4N2X8Lt.png" style="max-width: 100.0%;max-height: 100.0%;">. His total score is equal to the sum of his scores for each problem. In addition, Kevin's total score gets increased by <span class="tex-span">100</span> points for each successful hack, but gets decreased by <span class="tex-span">50</span> points for each unsuccessful hack.</p><p>All arithmetic operations are performed with absolute precision and no rounding. It is guaranteed that Kevin's final score is an integer.</p></div><div class="input-specification"><p>The first line of the input contains five space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">5</sub></span>, where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 119</span>) is the time of Kevin's last submission for problem <span class="tex-span"><i>i</i></span>. His last submission is always correct and gets accepted.</p><p>The second line contains five space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">5</sub></span>, where <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>) is Kevin's number of wrong submissions on problem <span class="tex-span"><i>i</i></span>.</p><p>The last line contains two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>u</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>s</i></sub>, <i>h</i><sub class="lower-index"><i>u</i></sub> ≤ 20</span>), denoting the Kevin's numbers of successful and unsuccessful hacks, respectively.</p></div><div class="output-specification"><p>Print a single integer, the value of Kevin's final score.</p></div>

## Input

<p>The first line of the input contains five space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">5</sub></span>, where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 119</span>) is the time of Kevin's last submission for problem <span class="tex-span"><i>i</i></span>. His last submission is always correct and gets accepted.</p><p>The second line contains five space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index">5</sub></span>, where <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>) is Kevin's number of wrong submissions on problem <span class="tex-span"><i>i</i></span>.</p><p>The last line contains two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>u</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>s</i></sub>, <i>h</i><sub class="lower-index"><i>u</i></sub> ≤ 20</span>), denoting the Kevin's numbers of successful and unsuccessful hacks, respectively.</p>

## Output

<p>Print a single integer, the value of Kevin's final score.</p>





```input1
20 40 60 80 100
0 1 2 3 4
1 0

```




```input2
119 119 119 119 119
0 0 0 0 0
10 0

```




```output1
4900

```




```output2
4930

```



## Note

<p>In the second sample, Kevin takes <span class="tex-span">119</span> minutes on all of the problems. Therefore, he gets <img align="middle" class="tex-formula" src="file://ztPtqpZb.png" style="max-width: 100.0%;max-height: 100.0%;"> of the points on each problem. So his score from solving problems is <img align="middle" class="tex-formula" src="file://FZOsFTd4.png" style="max-width: 100.0%;max-height: 100.0%;">. Adding in <span class="tex-span">10·100 = 1000</span> points from hacks, his total score becomes <span class="tex-span">3930 + 1000 = 4930</span>.</p>
