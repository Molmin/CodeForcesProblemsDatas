## Description

<div><p>You are looking at the floor plan of the Summer Informatics School's new building. You were tasked with SIS logistics, so you really care about travel time between different locations: it is important to know how long it would take to get from the lecture room to the canteen, or from the gym to the server room.</p><p>The building consists of <span class="tex-span"><i>n</i></span> towers, <span class="tex-span"><i>h</i></span> floors each, where the towers are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the floors are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>h</i></span>. There is a passage between any two adjacent towers (two towers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> for all <span class="tex-span"><i>i</i></span>: <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) on every floor <span class="tex-span"><i>x</i></span>, where <span class="tex-span"><i>a</i> ≤ <i>x</i> ≤ <i>b</i></span>. It takes exactly one minute to walk between any two adjacent floors of a tower, as well as between any two adjacent towers, provided that there is a passage on that floor. It is not permitted to leave the building.</p><center> <img class="tex-graphics" height="208px" src="file://xWVXPwba.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"><p><span class="tex-font-size-small">The picture illustrates the first example.</span> </p></center><p>You have given <span class="tex-span"><i>k</i></span> pairs of locations <span class="tex-span">(<i>t</i><sub class="lower-index"><i>a</i></sub>, <i>f</i><sub class="lower-index"><i>a</i></sub>)</span>, <span class="tex-span">(<i>t</i><sub class="lower-index"><i>b</i></sub>, <i>f</i><sub class="lower-index"><i>b</i></sub>)</span>: floor <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> of tower <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span> and floor <span class="tex-span"><i>f</i><sub class="lower-index"><i>b</i></sub></span> of tower <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>. For each pair you need to determine the minimum walking time between these locations.</p></div><div class="input-specification"><p>The first line of the input contains following integers:</p><ul> <li> <span class="tex-span"><i>n</i></span>: the number of towers in the building (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>), </li><li> <span class="tex-span"><i>h</i></span>: the number of floors in each tower (<span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup></span>), </li><li> <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>: the lowest and highest floor where it's possible to move between adjacent towers (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>h</i></span>), </li><li> <span class="tex-span"><i>k</i></span>: total number of queries (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>). </li></ul><p>Next <span class="tex-span"><i>k</i></span> lines contain description of the queries. Each description consists of four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>a</i></sub>, <i>t</i><sub class="lower-index"><i>b</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>a</i></sub>, <i>f</i><sub class="lower-index"><i>b</i></sub> ≤ <i>h</i></span>). This corresponds to a query to find the minimum travel time between <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span>-th floor of the <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span>-th tower and <span class="tex-span"><i>f</i><sub class="lower-index"><i>b</i></sub></span>-th floor of the <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>-th tower.</p></div><div class="output-specification"><p>For each query print a single integer: the minimum walking time between the locations in minutes.</p></div>

## Input

<p>The first line of the input contains following integers:</p><ul> <li> <span class="tex-span"><i>n</i></span>: the number of towers in the building (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>), </li><li> <span class="tex-span"><i>h</i></span>: the number of floors in each tower (<span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup></span>), </li><li> <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>: the lowest and highest floor where it's possible to move between adjacent towers (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>h</i></span>), </li><li> <span class="tex-span"><i>k</i></span>: total number of queries (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>). </li></ul><p>Next <span class="tex-span"><i>k</i></span> lines contain description of the queries. Each description consists of four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>a</i></sub>, <i>t</i><sub class="lower-index"><i>b</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>a</i></sub>, <i>f</i><sub class="lower-index"><i>b</i></sub> ≤ <i>h</i></span>). This corresponds to a query to find the minimum travel time between <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span>-th floor of the <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span>-th tower and <span class="tex-span"><i>f</i><sub class="lower-index"><i>b</i></sub></span>-th floor of the <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>-th tower.</p>

## Output

<p>For each query print a single integer: the minimum walking time between the locations in minutes.</p>





```input1
3 6 2 3 3
1 2 1 3
1 4 3 4
1 2 2 3

```




```output1
1
4
2

```


