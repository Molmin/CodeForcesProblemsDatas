## Description

<div><p>Gosha's universe is a table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Both the rows and columns are numbered with consecutive integers starting with <span class="tex-span">1</span>. We will use <span class="tex-span">(<i>r</i>, <i>c</i>)</span> to denote a cell located in the row <span class="tex-span"><i>r</i></span> and column <span class="tex-span"><i>c</i></span>.</p><p>Gosha is often invited somewhere. Every time he gets an invitation, he first calculates the number of ways to get to this place, and only then he goes. Gosha's house is located in the cell <span class="tex-span">(1, 1)</span>.</p><p>At any moment of time, Gosha moves from the cell he is currently located in to a cell adjacent to it (two cells are adjacent if they share a common side). Of course, the movement is possible only if such a cell exists, i.e. Gosha will not go beyond the boundaries of the table. Thus, from the cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> he is able to make a move to one of the cells <span class="tex-span">(<i>r</i> - 1, <i>c</i>)</span>, <span class="tex-span">(<i>r</i>, <i>c</i> - 1)</span>, <span class="tex-span">(<i>r</i> + 1, <i>c</i>)</span>, <span class="tex-span">(<i>r</i>, <i>c</i> + 1)</span>. Also, Ghosha can skip a move and stay in the current cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span>.</p><p>Besides the love of strange calculations, Gosha is allergic to cats, so he never goes to the cell that has a cat in it. Gosha knows exactly where and when he will be invited and the schedule of cats travelling along the table. Formally, he has <span class="tex-span"><i>q</i></span> records, the <span class="tex-span"><i>i</i></span>-th of them has one of the following forms: </p><ul> <li> <span class="tex-span">1</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— Gosha is invited to come to cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there is no cat inside cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at this moment of time. </li><li> <span class="tex-span">2</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> a cat appears in cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. It is guaranteed that no other cat is located in this cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at that moment of time. </li><li> <span class="tex-span">3</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> a cat leaves cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. It is guaranteed that there is cat located in the cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. </li></ul><p>Gosha plans to accept only one invitation, but he has not yet decided, which particular one. In order to make this decision, he asks you to calculate for each of the invitations <span class="tex-span"><i>i</i></span> the number of ways to get to the cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. For every invitation, assume that Gosha he starts moving from cell <span class="tex-span">(1, 1)</span> at the moment <span class="tex-span">1</span>.</p><p>Moving between two neighboring cells takes Gosha exactly one unit of tim. In particular, this means that Gosha can come into the cell only if a cat sitting in it leaves the moment when Gosha begins his movement from the neighboring cell, and if none of the cats comes to the cell at the time when Gosha is in it.</p><p>Two ways to go from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> at time <span class="tex-span"><i>t</i></span> are considered distinct if for at least one moment of time from <span class="tex-span">1</span> to <span class="tex-span"><i>t</i></span> Gosha's positions are distinct for the two ways at this moment. Note, that during this travel Gosha is allowed to visit both <span class="tex-span">(1, 1)</span> and <span class="tex-span">(<i>x</i>, <i>y</i>)</span> multiple times. Since the number of ways can be quite large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>·<i>m</i> ≤ 20, 1 ≤ <i>q</i> ≤ 10 000</span>) — the number of rows and columns in the table and the number of events respectively.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the events, each description contains four integers <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>tp</i> ≤ 3, 1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>, 2 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the type of the event (<span class="tex-span">1</span> if Gosha gets an invitation, <span class="tex-span">2</span> if a cat comes to the cell and <span class="tex-span">3</span> if a cat leaves the cell), the coordinates of the cell where the action takes place and the moment of time at which the action takes place respectively.</p><p>It is guaranteed that the queries are given in the chronological order, i.e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </p></div><div class="output-specification"><p>For each invitation <span class="tex-span"><i>i</i></span> (that is, <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub> = 1</span>) calculate the number of ways to get to cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Respond to the invitations chronologically, that is, in the order they appear in the input.</p></div>

## Input

<p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>·<i>m</i> ≤ 20, 1 ≤ <i>q</i> ≤ 10 000</span>) — the number of rows and columns in the table and the number of events respectively.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the events, each description contains four integers <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>tp</i> ≤ 3, 1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>, 2 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the type of the event (<span class="tex-span">1</span> if Gosha gets an invitation, <span class="tex-span">2</span> if a cat comes to the cell and <span class="tex-span">3</span> if a cat leaves the cell), the coordinates of the cell where the action takes place and the moment of time at which the action takes place respectively.</p><p>It is guaranteed that the queries are given in the chronological order, i.e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </p>

## Output

<p>For each invitation <span class="tex-span"><i>i</i></span> (that is, <span class="tex-span"><i>tp</i><sub class="lower-index"><i>i</i></sub> = 1</span>) calculate the number of ways to get to cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Respond to the invitations chronologically, that is, in the order they appear in the input.</p>





```input1
1 3 3
2 1 2 3
3 1 2 5
1 1 1 7

```




```input2
3 3 3
2 2 2 2
1 3 3 5
1 3 3 7

```




```input3
4 5 5
2 2 5 3
2 2 4 6
3 2 4 9
1 4 4 13
1 4 4 15

```




```output1
5

```




```output2
2
42

```




```output3
490902
10598759

```



## Note

<p>Explanation of the first sample. Each picture specifies the number of ways to arrive at the cell at the appropriate time. (X stands for a cell blocked at this particular moment of time)</p><center> <img class="tex-graphics" src="file://GobbyGa7.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 1. <center> <img class="tex-graphics" src="file://Io6IOad7.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 2.<center> <img class="tex-graphics" src="file://JnpMN9yO.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 3.<center> <img class="tex-graphics" src="file://Kiks1UUB.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 4.<center> <img class="tex-graphics" src="file://zKh6K4iF.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 5.<center> <img class="tex-graphics" src="file://nj14n4yp.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 6.<center> <img class="tex-graphics" src="file://Dk7uqb1G.png" style="max-width: 100.0%;max-height: 100.0%;"> Time moment 7.</center></center></center></center></center></center></center>
