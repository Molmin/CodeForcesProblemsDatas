## Description

<div><p>Some country consists of <span class="tex-span">(<i>n</i> + 1)</span> cities, located along a straight highway. Let's number the cities with consecutive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> + 1</span> in the order they occur along the highway. Thus, the cities are connected by <span class="tex-span"><i>n</i></span> segments of the highway, the <span class="tex-span"><i>i</i></span>-th segment connects cities number <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span>. Every segment of the highway is associated with a positive integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 1</span> — the period of traffic jams appearance on it. </p><p>In order to get from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>), some drivers use the following tactics. </p><p>Initially the driver is in city <span class="tex-span"><i>x</i></span> and the current time <span class="tex-span"><i>t</i></span> equals zero. Until the driver arrives in city <span class="tex-span"><i>y</i></span>, he perfors the following actions:</p><ul> <li> if the current time <span class="tex-span"><i>t</i></span> is a multiple of <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span>, then the segment of the highway number <span class="tex-span"><i>x</i></span> is now having traffic problems and the driver stays in the current city for one unit of time (formally speaking, we assign <span class="tex-span"><i>t</i> = <i>t</i> + 1</span>); </li><li> if the current time <span class="tex-span"><i>t</i></span> is not a <span class="tex-font-style-bf">multiple</span> of <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span>, then the segment of the highway number <span class="tex-span"><i>x</i></span> is now clear and that's why the driver uses one unit of time to move to city <span class="tex-span"><i>x</i> + 1</span> (formally, we assign <span class="tex-span"><i>t</i> = <i>t</i> + 1</span> and <span class="tex-span"><i>x</i> = <i>x</i> + 1</span>). </li></ul><p>You are developing a new traffic control system. You want to consecutively process <span class="tex-span"><i>q</i></span> queries of two types:</p><ol> <li> determine the final value of time <span class="tex-span"><i>t</i></span> after the ride from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>) assuming that we apply the tactics that is described above. Note that for each query <span class="tex-span"><i>t</i></span> is being reset to <span class="tex-span">0</span>. </li><li> replace the period of traffic jams appearing on the segment number <span class="tex-span"><i>x</i></span> by value <span class="tex-span"><i>y</i></span> (formally, assign <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> = <i>y</i></span>). </li></ol><p>Write a code that will effectively process the queries given above.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of highway segments that connect the <span class="tex-span"><i>n</i> + 1</span> cities.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>) — the periods of traffic jams appearance on segments of the highway.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries to process.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the queries in the format <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>c</i></span> — the query type). </p><p>If <span class="tex-span"><i>c</i></span> is character '<span class="tex-font-style-tt">A</span>', then your task is to process a query of the first type. In this case the following constraints are satisfied: <span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i> + 1</span>.</p><p>If <span class="tex-span"><i>c</i></span> is character '<span class="tex-font-style-tt">C</span>', then you need to process a query of the second type. In such case, the following constraints are satisfied: <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">2 ≤ <i>y</i> ≤ 6</span>.</p></div><div class="output-specification"><p>For each query of the first type output a single integer — the final value of time <span class="tex-span"><i>t</i></span> after driving from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span>. Process the queries in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of highway segments that connect the <span class="tex-span"><i>n</i> + 1</span> cities.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>) — the periods of traffic jams appearance on segments of the highway.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries to process.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the queries in the format <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>c</i></span> — the query type). </p><p>If <span class="tex-span"><i>c</i></span> is character '<span class="tex-font-style-tt">A</span>', then your task is to process a query of the first type. In this case the following constraints are satisfied: <span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i> + 1</span>.</p><p>If <span class="tex-span"><i>c</i></span> is character '<span class="tex-font-style-tt">C</span>', then you need to process a query of the second type. In such case, the following constraints are satisfied: <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">2 ≤ <i>y</i> ≤ 6</span>.</p>

## Output

<p>For each query of the first type output a single integer — the final value of time <span class="tex-span"><i>t</i></span> after driving from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span>. Process the queries in the order in which they are given in the input.</p>





```input1
10
2 5 3 2 3 5 3 4 2 4
10
C 10 6
A 2 6
A 1 3
C 3 4
A 3 11
A 4 9
A 5 6
C 7 3
A 8 10
A 2 5

```




```output1
5
3
14
6
2
4
4

```


