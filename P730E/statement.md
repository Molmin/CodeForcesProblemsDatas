## Description

<div><p>All-Berland programming contest comes to an end. In total, <span class="tex-span"><i>n</i></span> teams participated in it. Like in ACM-ICPC, current results stopped refreshing one hour before the contest ends. So at the Award Ceremony, results are partially known. For each team the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is given — the number of points the <span class="tex-span"><i>i</i></span>-th team has earned before the last hour of the contest. Besides that, the Jury has evaluated all submissions sent during the last hour and knows values <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of points earned by the <span class="tex-span"><i>i</i></span>-th team during the last hour (these values can be negative, which means that a team can lose points).</p><p>Before the contest, each team got unique id from 1 to <span class="tex-span"><i>n</i></span>. According to the contest rules, a team with more points takes a higher place. If two or more teams have equal number of points, the team with lower id will take the higher place. So no two teams can share the same place.</p><p>The Award Ceremony proceeds in the following way. At the beginning of the ceremony, a large screen shows the results for the time moment "one hour before the end", which means that the <span class="tex-span"><i>i</i></span>-th team has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> points. Then the Jury unfreezes results of the teams one by one in some order. When result of the <span class="tex-span"><i>j</i></span>-th team is unfrozen, its score changes from <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> + <i>d</i><sub class="lower-index"><i>j</i></sub></span>. At this time the table of results is modified and the place of the team can change. The unfreezing of the <span class="tex-span"><i>j</i></span>-th team is followed by the applause from the audience with duration of <span class="tex-span">|<i>x</i><sub class="lower-index"><i>j</i></sub> - <i>y</i><sub class="lower-index"><i>j</i></sub>|</span> seconds, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> is the place of the <span class="tex-span"><i>j</i></span>-th team before unfreezing and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> is the place right after the unfreezing. For example, if the team does not change the place, there is no applause from the audience. As you can see, during the Award Ceremony, each team will be unfrozen exactly once.</p><p>Your task is to find such an order to unfreeze all the teams that the total duration of applause is maximum possible.</p></div><div class="input-specification"><p>The first line of the input file contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of teams.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span"> - 100 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of points the <span class="tex-span"><i>i</i></span>-th team has earned before the last hour of the contest and the number of points earned by this team during the last hour. It is possible that after unfreezing a team will have a negative score.</p></div><div class="output-specification"><p>Print the only integer — maximal total applause duration in seconds if the Jury can choose any order of the teams to unfreeze.</p></div>

## Input

<p>The first line of the input file contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of teams.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span"> - 100 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of points the <span class="tex-span"><i>i</i></span>-th team has earned before the last hour of the contest and the number of points earned by this team during the last hour. It is possible that after unfreezing a team will have a negative score.</p>

## Output

<p>Print the only integer — maximal total applause duration in seconds if the Jury can choose any order of the teams to unfreeze.</p>





```input1
4
17 -14
52 -5
1 52
6 0

```




```input2
5
4 5
3 2
5 -3
6 -2
4 3

```




```output1
4

```




```output2
14

```



## Note

<p>In the first example the initial standings are:</p><ol> <li> Team 2, 52 points </li><li> Team 1, 17 points </li><li> Team 4, 6 points </li><li> Team 3, 1 point </li></ol><p>Here any order of unfreezing the teams leads to 4 seconds of applause in total. For example, let's unfreeze teams in their order from the Team 1 to the Team 4.</p><p>After the Team 1 became unfrozen the standings are:</p><ol> <li> Team 2, 52 points </li><li> Team 4, 6 points </li><li> Team 1, 3 points </li><li> Team 3, 1 point </li></ol><p>So there is 1 second of applause, because the difference between old and new places <span class="tex-span">|2 - 3| = 1</span>.</p><p>After the Team 2 became unfrozen the standings are:</p><ol> <li> Team 2, 47 points </li><li> Team 4, 6 points </li><li> Team 1, 3 points </li><li> Team 3, 1 point </li></ol><p>The place of the Team 2 has not changed, so no applause during unfreezing.</p><p>After the Team 3 became unfrozen the standings are:</p><ol> <li> Team 3, 53 point </li><li> Team 2, 47 points </li><li> Team 4, 6 points </li><li> Team 1, 3 points </li></ol><p>The place of the Team 3 has changed from 4 to 1, so the duration of applause is <span class="tex-span">|4 - 1| = 3</span>.</p><p>The unfreezing of the Team 4 has not changed any place because <span class="tex-span"><i>d</i><sub class="lower-index">4</sub> = 0</span>.</p><p>Therefore, the total duration of applause is <span class="tex-span">1 + 0 + 3 + 0 = 4</span> seconds.</p>
