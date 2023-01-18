## Description

<div><p>LiLand is a country, consisting of <span class="tex-span"><i>n</i></span> cities. The cities are numbered from 1 to <span class="tex-span"><i>n</i></span>. The country is well known because it has a very strange transportation system. There are many one-way flights that make it possible to travel between the cities, but the flights are arranged in a way that once you leave a city you will never be able to return to that city again.</p><p>Previously each flight took exactly one hour, but recently Lily has become the new manager of transportation system and she wants to change the duration of some flights. Specifically, she wants to change the duration of some flights to exactly 2 hours in such a way that all trips from city 1 to city <span class="tex-span"><i>n</i></span> take the same time regardless of their path.</p><p>Your task is to help Lily to change the duration of flights.</p></div><div class="input-specification"><p>First line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000;&nbsp;1 ≤ <i>m</i> ≤ 5000)</span> specifying the number of cities and the number of flights.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> specifying a one-directional flight from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there exists a way to travel from city number 1 to city number <span class="tex-span"><i>n</i></span> using the given flights. It is guaranteed that there is no sequence of flights that forms a cyclical path and no two flights are between the same pair of cities.</p></div><div class="output-specification"><p>If it is impossible for Lily to do her task, print "<span class="tex-font-style-tt">No</span>" (without quotes) on the only line of the output. </p><p>Otherwise print "<span class="tex-font-style-tt">Yes</span>" (without quotes) on the first line of output, then print an integer <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>ans</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span> to each of the next <span class="tex-span"><i>m</i></span> lines being the duration of flights in new transportation system. You should print these numbers in the order that flights are given in the input.</p><p>If there are multiple solutions for the input, output any of them.</p></div>

## Input

<p>First line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000;&nbsp;1 ≤ <i>m</i> ≤ 5000)</span> specifying the number of cities and the number of flights.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> specifying a one-directional flight from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there exists a way to travel from city number 1 to city number <span class="tex-span"><i>n</i></span> using the given flights. It is guaranteed that there is no sequence of flights that forms a cyclical path and no two flights are between the same pair of cities.</p>

## Output

<p>If it is impossible for Lily to do her task, print "<span class="tex-font-style-tt">No</span>" (without quotes) on the only line of the output. </p><p>Otherwise print "<span class="tex-font-style-tt">Yes</span>" (without quotes) on the first line of output, then print an integer <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>ans</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span> to each of the next <span class="tex-span"><i>m</i></span> lines being the duration of flights in new transportation system. You should print these numbers in the order that flights are given in the input.</p><p>If there are multiple solutions for the input, output any of them.</p>





```input1
3 3
1 2
2 3
1 3

```




```input2
4 4
1 2
2 3
3 4
1 4

```




```input3
5 6
1 2
2 3
3 5
1 4
4 5
1 3

```




```output1
Yes
1
1
2

```




```output2
No

```




```output3
Yes
1
1
1
2
1
2

```


