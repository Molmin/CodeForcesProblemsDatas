## Description

<div><p>Recently, Mike was very busy with studying for exams and contests. Now he is going to chill a bit by doing some sight seeing in the city.</p><p>City consists of <span class="tex-span"><i>n</i></span> intersections numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Mike starts walking from his house located at the intersection number <span class="tex-span">1</span> and goes along some sequence of intersections. Walking from intersection number <span class="tex-span"><i>i</i></span> to intersection <span class="tex-span"><i>j</i></span> requires <span class="tex-span">|<i>i</i> - <i>j</i>|</span> units of energy. The <span class="tex-font-style-it">total energy</span> spent by Mike to visit a sequence of intersections <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 1, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> is equal to <img align="middle" class="tex-formula" src="file://rkOnQ1yB.png" style="max-width: 100.0%;max-height: 100.0%;"> units of energy.</p><p>Of course, walking would be boring if there were no shortcuts. A <span class="tex-font-style-it">shortcut</span> is a special path that allows Mike walking from one intersection to another requiring only <span class="tex-span">1</span> unit of energy. There are exactly <span class="tex-span"><i>n</i></span> shortcuts in Mike's city, the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them allows walking from intersection <span class="tex-span"><i>i</i></span> to intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>i</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>) (but not in the opposite direction), thus there is exactly one shortcut starting at each intersection. Formally, if Mike chooses a sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 1, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> then for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span> satisfying <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub> ≠ <i>p</i><sub class="lower-index"><i>i</i></sub></span> Mike will spend <span class="tex-font-style-bf">only <span class="tex-span">1</span> unit of energy</span> instead of <span class="tex-span">|<i>p</i><sub class="lower-index"><i>i</i></sub> - <i>p</i><sub class="lower-index"><i>i</i> + 1</sub>|</span> walking from the intersection <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>. For example, if Mike chooses a sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 1, <i>p</i><sub class="lower-index">2</sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub>, <i>p</i><sub class="lower-index">3</sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub> = <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>k</i> - 1</sub></sub></span>, he spends exactly <span class="tex-span"><i>k</i> - 1</span> units of total energy walking around them.</p><p>Before going on his adventure, Mike asks you to find the minimum amount of energy required to reach each of the intersections from his home. Formally, for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span> Mike is interested in finding minimum possible total energy of some sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 1, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub> = <i>i</i></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of Mike's city intersection.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>i</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> , <img align="middle" class="tex-formula" src="file://n2CfjOfH.png" style="max-width: 100.0%;max-height: 100.0%;">, describing shortcuts of Mike's city, allowing to walk from intersection <span class="tex-span"><i>i</i></span> to intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> using only <span class="tex-span">1</span> unit of energy. Please note that the shortcuts don't allow walking in opposite directions (from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>i</i></span>).</p></div><div class="output-specification"><p>In the only line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> denotes the least amount of total energy required to walk from intersection <span class="tex-span">1</span> to intersection <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of Mike's city intersection.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>i</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> , <img align="middle" class="tex-formula" src="file://n2CfjOfH.png" style="max-width: 100.0%;max-height: 100.0%;">, describing shortcuts of Mike's city, allowing to walk from intersection <span class="tex-span"><i>i</i></span> to intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> using only <span class="tex-span">1</span> unit of energy. Please note that the shortcuts don't allow walking in opposite directions (from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>i</i></span>).</p>

## Output

<p>In the only line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> denotes the least amount of total energy required to walk from intersection <span class="tex-span">1</span> to intersection <span class="tex-span"><i>i</i></span>.</p>





```input1
3
2 2 3

```




```input2
5
1 2 3 4 5

```




```input3
7
4 4 4 4 7 7 7

```




```output1
0 1 2 

```




```output2
0 1 2 3 4 

```




```output3
0 1 2 1 2 3 3 

```



## Note

<p>In the first sample case desired sequences are:</p><p><span class="tex-span">1: 1</span>; <span class="tex-span"><i>m</i><sub class="lower-index">1</sub> = 0</span>;</p><p><span class="tex-span">2: 1, 2</span>; <span class="tex-span"><i>m</i><sub class="lower-index">2</sub> = 1</span>;</p><p><span class="tex-span">3: 1, 3</span>; <span class="tex-span"><i>m</i><sub class="lower-index">3</sub> = |3 - 1| = 2</span>.</p><p>In the second sample case the sequence for any intersection <span class="tex-span">1 &lt; <i>i</i></span> is always <span class="tex-span">1, <i>i</i></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub> = |1 - <i>i</i>|</span>.</p><p>In the third sample case&nbsp;— consider the following intersection sequences:</p><p><span class="tex-span">1: 1</span>; <span class="tex-span"><i>m</i><sub class="lower-index">1</sub> = 0</span>;</p><p><span class="tex-span">2: 1, 2</span>; <span class="tex-span"><i>m</i><sub class="lower-index">2</sub> = |2 - 1| = 1</span>;</p><p><span class="tex-span">3: 1, 4, 3</span>; <span class="tex-span"><i>m</i><sub class="lower-index">3</sub> = 1 + |4 - 3| = 2</span>;</p><p><span class="tex-span">4: 1, 4</span>; <span class="tex-span"><i>m</i><sub class="lower-index">4</sub> = 1</span>;</p><p><span class="tex-span">5: 1, 4, 5</span>; <span class="tex-span"><i>m</i><sub class="lower-index">5</sub> = 1 + |4 - 5| = 2</span>;</p><p><span class="tex-span">6: 1, 4, 6</span>; <span class="tex-span"><i>m</i><sub class="lower-index">6</sub> = 1 + |4 - 6| = 3</span>;</p><p><span class="tex-span">7: 1, 4, 5, 7</span>; <span class="tex-span"><i>m</i><sub class="lower-index">7</sub> = 1 + |4 - 5| + 1 = 3</span>.</p>
