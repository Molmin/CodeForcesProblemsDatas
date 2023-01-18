## Description

<div><p>Bizon the Champion has recently finished painting his wood fence. The fence consists of a sequence of <span class="tex-span"><i>n</i></span> panels of <span class="tex-span">1</span> meter width and of arbitrary height. The <span class="tex-span"><i>i</i></span>-th panel's height is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> meters. The adjacent planks follow without a gap between them.</p><p>After Bizon painted the fence he decided to put a "for sale" sign on it. The sign will be drawn on a rectangular piece of paper and placed on the fence so that the sides of the sign are parallel to the fence panels and are also aligned with the edges of some panels. Bizon the Champion introduced the following constraints for the sign position:</p><ol> <li> The width of the sign should be exactly <span class="tex-span"><i>w</i></span> meters. </li><li> The sign must fit into the segment of the fence from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th panels, inclusive (also, it can't exceed the fence's bound in vertical direction). </li></ol><p>The sign will be really pretty, So Bizon the Champion wants the sign's height to be as large as possible.</p><p>You are given the description of the fence and several queries for placing sign. For each query print the maximum possible height of the sign that can be placed on the corresponding segment of the fence with the given fixed width of the sign.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of panels in the fence (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>,&nbsp;— the heights of the panels (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>The third line contains an integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of the queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries, each query is represented by three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ <i>r</i> - <i>l</i> + 1</span>)&nbsp;— the segment of the fence and the width of the sign respectively.</p></div><div class="output-specification"><p>For each query print the answer on a separate line&nbsp;— the maximum height of the sign that can be put in the corresponding segment of the fence with all the conditions being satisfied.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of panels in the fence (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>,&nbsp;— the heights of the panels (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>The third line contains an integer <span class="tex-span"><i>m</i></span>&nbsp;— the number of the queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries, each query is represented by three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ <i>r</i> - <i>l</i> + 1</span>)&nbsp;— the segment of the fence and the width of the sign respectively.</p>

## Output

<p>For each query print the answer on a separate line&nbsp;— the maximum height of the sign that can be put in the corresponding segment of the fence with all the conditions being satisfied.</p>





```input1
5
1 2 2 3 3
3
2 5 3
2 5 2
1 5 5

```




```output1
2
3
1

```



## Note

<p>The fence described in the sample looks as follows: </p><center> <img class="tex-graphics" src="file://nFmjmiia.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The possible positions for the signs for all queries are given below.</p><center> <img class="tex-graphics" src="file://TEOY2jIs.png" style="max-width: 100.0%;max-height: 100.0%;"> The optimal position of the sign for the first query. </center><center> <img class="tex-graphics" src="file://sbBdOL3X.png" style="max-width: 100.0%;max-height: 100.0%;"> The optimal position of the sign for the second query. </center><center> <img class="tex-graphics" src="file://sPPQSfSF.png" style="max-width: 100.0%;max-height: 100.0%;"> The optimal position of the sign for the third query. </center>
