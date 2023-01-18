## Description

<div><p>Innovation technologies are on a victorious march around the planet. They integrate into all spheres of human activity!</p><p>A restaurant called "Dijkstra's Place" has started thinking about optimizing the booking system. </p><p>There are <span class="tex-span"><i>n</i></span> booking requests received by now. Each request is characterized by two numbers: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the size of the group of visitors who will come via this request and the total sum of money they will spend in the restaurant, correspondingly.</p><p>We know that for each request, all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> people want to sit at the same table and are going to spend the whole evening in the restaurant, from the opening moment at 18:00 to the closing moment.</p><p>Unfortunately, there only are <span class="tex-span"><i>k</i></span> tables in the restaurant. For each table, we know <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the maximum number of people who can sit at it. A table can have only people from the same group sitting at it. If you cannot find a large enough table for the whole group, then all visitors leave and naturally, pay nothing.</p><p>Your task is: given the tables and the requests, decide which requests to accept and which requests to decline so that the money paid by the happy and full visitors was maximum.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of requests from visitors. Then <span class="tex-span"><i>n</i></span> lines follow. Each line contains two integers: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the size of the group of visitors who will come by the <span class="tex-span"><i>i</i></span>-th request and the total sum of money they will pay when they visit the restaurant, correspondingly.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of tables in the restaurant. The last line contains <span class="tex-span"><i>k</i></span> space-separated integers: <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the maximum number of people that can sit at each table.</p></div><div class="output-specification"><p>In the first line print two integers: <span class="tex-span"><i>m</i>, <i>s</i></span> — the number of accepted requests and the total money you get from these requests, correspondingly.</p><p>Then print <span class="tex-span"><i>m</i></span> lines — each line must contain two space-separated integers: the number of the accepted request and the number of the table to seat people who come via this request. The requests and the tables are consecutively numbered starting from <span class="tex-span">1</span> in the order in which they are given in the input.</p><p>If there are multiple optimal answers, print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of requests from visitors. Then <span class="tex-span"><i>n</i></span> lines follow. Each line contains two integers: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the size of the group of visitors who will come by the <span class="tex-span"><i>i</i></span>-th request and the total sum of money they will pay when they visit the restaurant, correspondingly.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of tables in the restaurant. The last line contains <span class="tex-span"><i>k</i></span> space-separated integers: <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the maximum number of people that can sit at each table.</p>

## Output

<p>In the first line print two integers: <span class="tex-span"><i>m</i>, <i>s</i></span> — the number of accepted requests and the total money you get from these requests, correspondingly.</p><p>Then print <span class="tex-span"><i>m</i></span> lines — each line must contain two space-separated integers: the number of the accepted request and the number of the table to seat people who come via this request. The requests and the tables are consecutively numbered starting from <span class="tex-span">1</span> in the order in which they are given in the input.</p><p>If there are multiple optimal answers, print any of them.</p>





```input1
3
10 50
2 100
5 30
3
4 6 9

```




```output1
2 130
2 1
3 2

```


