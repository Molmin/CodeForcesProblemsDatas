## Description

<div><p>In Berland each feudal owns exactly one castle and each castle belongs to exactly one feudal.</p><p>Each feudal, except one (the King) is subordinate to another feudal. A feudal can have any number of vassals (subordinates).</p><p>Some castles are connected by roads, it is allowed to move along the roads in both ways. Two castles have a road between them if and only if the owner of one of these castles is a direct subordinate to the other owner.</p><p>Each year exactly one of these two events may happen in Berland.</p><ol> <li> The barbarians attacked castle <span class="tex-span"><i>c</i></span>. The interesting fact is, the barbarians never attacked the same castle twice throughout the whole Berlandian history. </li><li> A noble knight sets off on a journey from castle <span class="tex-span"><i>a</i></span> to castle <span class="tex-span"><i>b</i></span> (provided that on his path he encounters each castle not more than once). </li></ol><p>Let's consider the second event in detail. As the journey from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> is not short, then the knight might want to stop at a castle he encounters on his way to have some rest. However, he can't stop at just any castle: his nobility doesn't let him stay in the castle that has been desecrated by the enemy's stench. A castle is desecrated if and only if it has been attacked after the year of <span class="tex-span"><i>y</i></span>. So, the knight chooses the <span class="tex-span"><i>k</i></span>-th castle he encounters, starting from <span class="tex-span"><i>a</i></span> (castles <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> aren't taken into consideration), that hasn't been attacked in years from <span class="tex-span"><i>y</i> + 1</span> till current year.</p><p>The knights don't remember which castles were attacked on what years, so he asked the court scholar, aka you to help them. You've got a sequence of events in the Berland history. Tell each knight, in what city he should stop or else deliver the sad news — that the path from city <span class="tex-span"><i>a</i></span> to city <span class="tex-span"><i>b</i></span> has less than <span class="tex-span"><i>k</i></span> cities that meet his requirements, so the knight won't be able to rest.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of feudals. </p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th integer shows either the number of the <span class="tex-span"><i>i</i></span>-th feudal's master, or a <span class="tex-span">0</span>, if the <span class="tex-span"><i>i</i></span>-th feudal is the King. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines that describe the events. The <span class="tex-span"><i>i</i></span>-th line (the lines are indexed starting from <span class="tex-span">1</span>) contains the description of the event that occurred in year <span class="tex-span"><i>i</i></span>. Each event is characterised by type <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. The description of the first type event looks as two space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>t</i><sub class="lower-index"><i>i</i></sub> = 1;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle that was attacked by the barbarians in the <span class="tex-span"><i>i</i></span>-th year. The description of the second type contains five space-separated integers: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>t</i><sub class="lower-index"><i>i</i></sub> = 2;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle from which the knight is setting off, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle to which the knight is going, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>y</i></span> from the second event's description.</p><p>You can consider the feudals indexed from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that there is only one king among the feudals. It is guaranteed that for the first type events all values <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are different.</p></div><div class="output-specification"><p>For each second type event print an integer — the number of the castle where the knight must stay to rest, or -1, if he will have to cover the distance from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> without a rest. Separate the answers by whitespaces.</p><p>Print the answers in the order, in which the second type events are given in the input.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of feudals. </p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th integer shows either the number of the <span class="tex-span"><i>i</i></span>-th feudal's master, or a <span class="tex-span">0</span>, if the <span class="tex-span"><i>i</i></span>-th feudal is the King. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines that describe the events. The <span class="tex-span"><i>i</i></span>-th line (the lines are indexed starting from <span class="tex-span">1</span>) contains the description of the event that occurred in year <span class="tex-span"><i>i</i></span>. Each event is characterised by type <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. The description of the first type event looks as two space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>t</i><sub class="lower-index"><i>i</i></sub> = 1;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle that was attacked by the barbarians in the <span class="tex-span"><i>i</i></span>-th year. The description of the second type contains five space-separated integers: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>t</i><sub class="lower-index"><i>i</i></sub> = 2;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle from which the knight is setting off, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of the castle to which the knight is going, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>y</i></span> from the second event's description.</p><p>You can consider the feudals indexed from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that there is only one king among the feudals. It is guaranteed that for the first type events all values <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are different.</p>

## Output

<p>For each second type event print an integer — the number of the castle where the knight must stay to rest, or -1, if he will have to cover the distance from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> without a rest. Separate the answers by whitespaces.</p><p>Print the answers in the order, in which the second type events are given in the input.</p>





```input1
3
0 1 2
5
2 1 3 1 0
1 2
2 1 3 1 0
2 1 3 1 1
2 1 3 1 2

```




```input2
6
2 5 2 2 0 5
3
2 1 6 2 0
1 2
2 4 5 1 0

```




```output1
2
-1
-1
2

```




```output2
5
-1

```



## Note

<p>In the first sample there is only castle <span class="tex-span">2</span> on the knight's way from castle <span class="tex-span">1</span> to castle <span class="tex-span">3</span>. When the knight covers the path <span class="tex-span">1 - 3</span> for the first time, castle <span class="tex-span">2</span> won't be desecrated by an enemy and the knight will stay there. In the second year the castle <span class="tex-span">2</span> will become desecrated, so the knight won't have anywhere to stay for the next two years (as finding a castle that hasn't been desecrated from years <span class="tex-span">1</span> and <span class="tex-span">2</span>, correspondingly, is important for him). In the fifth year the knight won't consider the castle <span class="tex-span">2</span> desecrated, so he will stay there again.</p>
