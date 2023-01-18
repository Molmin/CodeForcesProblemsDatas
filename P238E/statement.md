## Description

<div><p>Urpal lives in a big city. He has planned to meet his lover tonight. </p><p>The city has <span class="tex-span"><i>n</i></span> junctions numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The junctions are connected by <span class="tex-span"><i>m</i></span> directed streets, all the roads have equal length. Urpal lives in junction <span class="tex-span"><i>a</i></span> and the date is planned in a restaurant in junction <span class="tex-span"><i>b</i></span>. He wants to use public transportation to get to junction <span class="tex-span"><i>b</i></span>. There are <span class="tex-span"><i>k</i></span> bus transportation companies. At the beginning of every second, a bus from the <span class="tex-span"><i>i</i></span>-th company chooses a random shortest path between junction <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and junction <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and passes through it. There might be no path from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. In that case no bus will leave from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. If a bus passes through a junction where Urpal stands, he can get on the bus. He can also get off the bus at any junction along the path. </p><p>Now Urpal wants to know if it's possible to go to the date using public transportation in a finite amount of time (the time of travel is the sum of length of the traveled roads) and what is the minimum number of buses he should take in the worst case.</p><p><span class="tex-font-style-bf">At any moment Urpal knows only his own position and the place where the date will be. When he gets on the bus he knows only the index of the company of this bus. Of course Urpal knows the city map and the the pairs <span class="tex-span">(<i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>)</span> for each company.</span></p><p>Note that Urpal doesn't know buses velocity. </p></div><div class="input-specification"><p>The first line of the input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100;&nbsp;0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1);&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>;&nbsp;<i>a</i> ≠ <i>b</i>)</span>. </p><p>The next <span class="tex-span"><i>m</i></span> lines contain two integers each <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> describing a directed road from junction <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to junction <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. All roads in the input will be distinct. </p><p>The next line contains an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 100)</span>. There will be <span class="tex-span"><i>k</i></span> lines after this, each containing two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub>)</span> saying there is a bus route starting at <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and ending at <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Please note that there might be no path from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, this case is described in the problem statement.</p></div><div class="output-specification"><p>In the only line of output print the minimum number of buses Urpal should get on on his way in the worst case. If it's not possible to reach the destination in the worst case print -1.</p></div>

## Input

<p>The first line of the input contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100;&nbsp;0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1);&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>;&nbsp;<i>a</i> ≠ <i>b</i>)</span>. </p><p>The next <span class="tex-span"><i>m</i></span> lines contain two integers each <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> describing a directed road from junction <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to junction <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. All roads in the input will be distinct. </p><p>The next line contains an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 100)</span>. There will be <span class="tex-span"><i>k</i></span> lines after this, each containing two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub>)</span> saying there is a bus route starting at <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and ending at <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Please note that there might be no path from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, this case is described in the problem statement.</p>

## Output

<p>In the only line of output print the minimum number of buses Urpal should get on on his way in the worst case. If it's not possible to reach the destination in the worst case print -1.</p>





```input1
7 8 1 7
1 2
1 3
2 4
3 4
4 6
4 5
6 7
5 7
3
2 7
1 4
5 7

```




```input2
4 4 1 2
1 2
1 3
2 4
3 4
1
1 4

```




```output1
2

```




```output2
-1

```


