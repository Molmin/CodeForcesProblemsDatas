## Description

<div><p>Gerda is travelling to the palace of the Snow Queen.</p><p>The road network consists of <span class="tex-span"><i>n</i></span> intersections and <span class="tex-span"><i>m</i></span> bidirectional roads. Roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Snow Queen put a powerful spell on the roads to change the weather conditions there. Now, if Gerda steps on the road <span class="tex-span"><i>i</i></span> at the moment of time less or equal to <span class="tex-span"><i>i</i></span>, she will leave the road exactly at the moment <span class="tex-span"><i>i</i></span>. In case she steps on the road <span class="tex-span"><i>i</i></span> at the moment of time greater than <span class="tex-span"><i>i</i></span>, she stays there forever.</p><p>Gerda starts at the moment of time <span class="tex-span"><i>l</i></span> at the intersection number <span class="tex-span"><i>s</i></span> and goes to the palace of the Snow Queen, located at the intersection number <span class="tex-span"><i>t</i></span>. Moreover, she has to be there at the moment <span class="tex-span"><i>r</i></span> (or earlier), before the arrival of the Queen.</p><p>Given the description of the road network, determine for <span class="tex-span"><i>q</i></span> queries <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> if it's possible for Gerda to get to the palace on time.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 200 000</span>)&nbsp;— the number of intersections in the road network of Snow Queen's Kingdom, the number of roads and the number of queries you have to answer.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains the description of the road number <span class="tex-span"><i>i</i></span>. The description consists of two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the indices of the intersections connected by the <span class="tex-span"><i>i</i></span>-th road. It's possible to get both from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> using only this road. Each pair of intersection may appear several times, meaning there are several roads connecting this pair.</p><p>Last <span class="tex-span"><i>q</i></span> lines contain the queries descriptions. Each of them consists of four integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the moment of time Gerda starts her journey, the last moment of time she is allowed to arrive to the palace, the index of the starting intersection and the index of the intersection where palace is located.</p></div><div class="output-specification"><p>For each query print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Gerda can be at the Snow Queen palace on time (not later than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>) or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 200 000</span>)&nbsp;— the number of intersections in the road network of Snow Queen's Kingdom, the number of roads and the number of queries you have to answer.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains the description of the road number <span class="tex-span"><i>i</i></span>. The description consists of two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the indices of the intersections connected by the <span class="tex-span"><i>i</i></span>-th road. It's possible to get both from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> using only this road. Each pair of intersection may appear several times, meaning there are several roads connecting this pair.</p><p>Last <span class="tex-span"><i>q</i></span> lines contain the queries descriptions. Each of them consists of four integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the moment of time Gerda starts her journey, the last moment of time she is allowed to arrive to the palace, the index of the starting intersection and the index of the intersection where palace is located.</p>

## Output

<p>For each query print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Gerda can be at the Snow Queen palace on time (not later than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>) or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
5 4 6
1 2
2 3
3 4
3 5
1 3 1 4
1 3 2 4
1 4 4 5
1 4 4 1
2 3 1 4
2 2 2 3

```




```output1
Yes
Yes
Yes
No
No
Yes

```


