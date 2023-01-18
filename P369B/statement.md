## Description

<div><p>Valera loves to participate in competitions. Especially in programming contests. Today he has participated in the contest with his team, consisting of <span class="tex-span"><i>n</i></span> students (including Valera). This contest was an individual competition, so each student in the team solved problems individually.</p><p>After the contest was over, Valera was interested in results. He found out that:</p><ul> <li> each student in the team scored at least <span class="tex-span"><i>l</i></span> points and at most <span class="tex-span"><i>r</i></span> points; </li><li> in total, all members of the team scored exactly <span class="tex-span"><i>s</i><sub class="lower-index"><i>all</i></sub></span> points; </li><li> the total score of the <span class="tex-span"><i>k</i></span> members of the team who scored the most points is equal to exactly <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span>; more formally, if <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is the sequence of points earned by the team of students in the non-increasing order <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub> ≥ <i>a</i><sub class="lower-index">2</sub> ≥ ... ≥ <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>, then <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>k</i></sub></span>. </li></ul><p>However, Valera did not find out exactly how many points each of <span class="tex-span"><i>n</i></span> students scored. Valera asked you to recover any distribution of scores between the students of the team, such that all the conditions above are met.</p></div><div class="input-specification"><p>The first line of the input contains exactly six integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>l</i>, <i>r</i>, <i>s</i><sub class="lower-index"><i>all</i></sub>, <i>s</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i>, <i>l</i>, <i>r</i> ≤ 1000</span>; <span class="tex-span"><i>l</i> ≤ <i>r</i></span>; <span class="tex-span"><i>k</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>k</i></sub> ≤ <i>s</i><sub class="lower-index"><i>all</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It's guaranteed that the input is such that the answer exists.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the number of points each student scored. If there are multiple solutions, you can print any of them. You can print the distribution of points in any order. </p></div>

## Input

<p>The first line of the input contains exactly six integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>l</i>, <i>r</i>, <i>s</i><sub class="lower-index"><i>all</i></sub>, <i>s</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i>, <i>l</i>, <i>r</i> ≤ 1000</span>; <span class="tex-span"><i>l</i> ≤ <i>r</i></span>; <span class="tex-span"><i>k</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>k</i></sub> ≤ <i>s</i><sub class="lower-index"><i>all</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It's guaranteed that the input is such that the answer exists.</p>

## Output

<p>Print exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the number of points each student scored. If there are multiple solutions, you can print any of them. You can print the distribution of points in any order. </p>





```input1
5 3 1 3 13 9

```




```input2
5 3 1 3 15 9

```




```output1
2 3 2 3 3
```




```output2
3 3 3 3 3
```


