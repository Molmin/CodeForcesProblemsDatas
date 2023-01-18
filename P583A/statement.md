## Description

<div><p>City X consists of <span class="tex-span"><i>n</i></span> vertical and <span class="tex-span"><i>n</i></span> horizontal infinite roads, forming <span class="tex-span"><i>n</i> × <i>n</i></span> intersections. Roads (both vertical and horizontal) are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the intersections are indicated by the numbers of the roads that form them.</p><p>Sand roads have long been recognized out of date, so the decision was made to asphalt them. To do this, a team of workers was hired and a schedule of work was made, according to which the intersections should be asphalted.</p><p>Road repairs are planned for <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> days. On the <span class="tex-span"><i>i</i></span>-th day of the team arrives at the <span class="tex-span"><i>i</i></span>-th intersection in the list and if <span class="tex-font-style-bf">none</span> of the two roads that form the intersection were already asphalted they asphalt both roads. Otherwise, the team leaves the intersection, without doing anything with the roads.</p><p>According to the schedule of road works tell in which days at least one road will be asphalted.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of vertical and horizontal roads in the city. </p><p>Next <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> lines contain the order of intersections in the schedule. The <span class="tex-span"><i>i</i></span>-th of them contains two numbers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), separated by a space, and meaning that the intersection that goes <span class="tex-span"><i>i</i></span>-th in the timetable is at the intersection of the <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>-th horizontal and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th vertical roads. It is guaranteed that all the intersections in the timetable are distinct.</p></div><div class="output-specification"><p>In the single line print the numbers of the days when road works will be in progress in ascending order. The days are numbered starting from <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of vertical and horizontal roads in the city. </p><p>Next <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> lines contain the order of intersections in the schedule. The <span class="tex-span"><i>i</i></span>-th of them contains two numbers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), separated by a space, and meaning that the intersection that goes <span class="tex-span"><i>i</i></span>-th in the timetable is at the intersection of the <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>-th horizontal and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th vertical roads. It is guaranteed that all the intersections in the timetable are distinct.</p>

## Output

<p>In the single line print the numbers of the days when road works will be in progress in ascending order. The days are numbered starting from <span class="tex-span">1</span>.</p>





```input1
2
1 1
1 2
2 1
2 2

```




```input2
1
1 1

```




```output1
1 4 

```




```output2
1 

```



## Note

<p>In the sample the brigade acts like that:</p><ol> <li> On the first day the brigade comes to the intersection of the 1-st horizontal and the 1-st vertical road. As none of them has been asphalted, the workers asphalt the 1-st vertical and the 1-st horizontal road; </li><li> On the second day the brigade of the workers comes to the intersection of the 1-st horizontal and the 2-nd vertical road. The 2-nd vertical road hasn't been asphalted, but as the 1-st horizontal road has been asphalted on the first day, the workers leave and do not asphalt anything; </li><li> On the third day the brigade of the workers come to the intersection of the 2-nd horizontal and the 1-st vertical road. The 2-nd horizontal road hasn't been asphalted but as the 1-st vertical road has been asphalted on the first day, the workers leave and do not asphalt anything; </li><li> On the fourth day the brigade come to the intersection formed by the intersection of the 2-nd horizontal and 2-nd vertical road. As none of them has been asphalted, the workers asphalt the 2-nd vertical and the 2-nd horizontal road. </li></ol>
