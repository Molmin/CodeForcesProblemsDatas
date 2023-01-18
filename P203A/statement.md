## Description

<div><p>A boy Valera registered on site <span class="tex-font-style-tt">Codeforces</span> as <span class="tex-font-style-tt">Valera</span>, and wrote his first <span class="tex-font-style-tt">Codeforces Round #300</span>. He boasted to a friend Arkady about winning as much as <span class="tex-span"><i>x</i></span> points for his first contest. But Arkady did not believe his friend's words and decided to check whether Valera could have shown such a result.</p><p>He knows that the contest number <span class="tex-span">300</span> was unusual because there were only two problems. The contest lasted for <span class="tex-span"><i>t</i></span> minutes, the minutes are numbered starting from zero. The first problem had the initial cost of <span class="tex-span"><i>a</i></span> points, and every minute its cost reduced by <span class="tex-span"><i>d</i><sub class="lower-index"><i>a</i></sub></span> points. The second problem had the initial cost of <span class="tex-span"><i>b</i></span> points, and every minute this cost reduced by <span class="tex-span"><i>d</i><sub class="lower-index"><i>b</i></sub></span> points. Thus, as soon as the zero minute of the contest is over, the first problem will cost <span class="tex-span"><i>a</i> - <i>d</i><sub class="lower-index"><i>a</i></sub></span> points, and the second problem will cost <span class="tex-span"><i>b</i> - <i>d</i><sub class="lower-index"><i>b</i></sub></span> points. It is guaranteed that at any moment of the contest each problem has a non-negative cost.</p><p>Arkady asks you to find out whether Valera could have got exactly <span class="tex-span"><i>x</i></span> points for this contest. You should assume that Valera could have solved any number of the offered problems. You should also assume that for each problem Valera made no more than one attempt, besides, he could have submitted both problems at the same minute of the contest, starting with minute <span class="tex-span">0</span> and ending with minute number <span class="tex-span"><i>t</i> - 1</span>. Please note that Valera can't submit a solution exactly <span class="tex-span"><i>t</i></span> minutes after the start of the contest or later.</p></div><div class="input-specification"><p>The single line of the input contains six integers <span class="tex-span"><i>x</i>, <i>t</i>, <i>a</i>, <i>b</i>, <i>d</i><sub class="lower-index"><i>a</i></sub>, <i>d</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i> ≤ 600;&nbsp;1 ≤ <i>t</i>, <i>a</i>, <i>b</i>, <i>d</i><sub class="lower-index"><i>a</i></sub>, <i>d</i><sub class="lower-index"><i>b</i></sub> ≤ 300)</span> — Valera's result, the contest's duration, the initial cost of the first problem, the initial cost of the second problem, the number of points that the first and the second problem lose per minute, correspondingly.</p><p>It is guaranteed that at each minute of the contest each problem has a non-negative cost, that is, <span class="tex-span"><i>a</i> - <i>i</i>·<i>d</i><sub class="lower-index"><i>a</i></sub> ≥ 0</span> and <span class="tex-span"><i>b</i> - <i>i</i>·<i>d</i><sub class="lower-index"><i>b</i></sub> ≥ 0</span> for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>t</i> - 1</span>.</p></div><div class="output-specification"><p>If Valera could have earned exactly <span class="tex-span"><i>x</i></span> points at a contest, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The single line of the input contains six integers <span class="tex-span"><i>x</i>, <i>t</i>, <i>a</i>, <i>b</i>, <i>d</i><sub class="lower-index"><i>a</i></sub>, <i>d</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i> ≤ 600;&nbsp;1 ≤ <i>t</i>, <i>a</i>, <i>b</i>, <i>d</i><sub class="lower-index"><i>a</i></sub>, <i>d</i><sub class="lower-index"><i>b</i></sub> ≤ 300)</span> — Valera's result, the contest's duration, the initial cost of the first problem, the initial cost of the second problem, the number of points that the first and the second problem lose per minute, correspondingly.</p><p>It is guaranteed that at each minute of the contest each problem has a non-negative cost, that is, <span class="tex-span"><i>a</i> - <i>i</i>·<i>d</i><sub class="lower-index"><i>a</i></sub> ≥ 0</span> and <span class="tex-span"><i>b</i> - <i>i</i>·<i>d</i><sub class="lower-index"><i>b</i></sub> ≥ 0</span> for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>t</i> - 1</span>.</p>

## Output

<p>If Valera could have earned exactly <span class="tex-span"><i>x</i></span> points at a contest, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
30 5 20 20 3 5

```




```input2
10 4 100 5 5 1

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample Valera could have acted like this: he could have submitted the first problem at minute <span class="tex-span">0</span> and the second problem — at minute <span class="tex-span">2</span>. Then the first problem brings him <span class="tex-span">20</span> points and the second problem brings him <span class="tex-span">10</span> points, that in total gives the required <span class="tex-span">30</span> points.</p>
