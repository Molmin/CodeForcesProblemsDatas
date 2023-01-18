## Description

<div><p>Recently Irina arrived to one of the most famous cities of Berland&nbsp;— the Berlatov city. There are <span class="tex-span"><i>n</i></span> showplaces in the city, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and some of them are connected by one-directional roads. The roads in Berlatov are designed in a way such that there <span class="tex-font-style-bf">are no</span> cyclic routes between showplaces.</p><p>Initially Irina stands at the showplace <span class="tex-span">1</span>, and the endpoint of her journey is the showplace <span class="tex-span"><i>n</i></span>. Naturally, Irina wants to visit as much showplaces as she can during her journey. However, Irina's stay in Berlatov is limited and she can't be there for more than <span class="tex-span"><i>T</i></span> time units.</p><p>Help Irina determine how many showplaces she may visit during her journey from showplace <span class="tex-span">1</span> to showplace <span class="tex-span"><i>n</i></span> within a time not exceeding <span class="tex-span"><i>T</i></span>. It is guaranteed that there is at least one route from showplace <span class="tex-span">1</span> to showplace <span class="tex-span"><i>n</i></span> such that Irina will spend no more than <span class="tex-span"><i>T</i></span> time units passing it.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000,  1 ≤ <i>m</i> ≤ 5000,  1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of showplaces, the number of roads between them and the time of Irina's stay in Berlatov respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines describes roads in Berlatov. <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span">3</span> integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), meaning that there is a road starting from showplace <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and leading to showplace <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and Irina spends <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> time units to pass it. It is guaranteed that the roads do not form cyclic routes.</p><p><span class="tex-font-style-bf">It is guaranteed, that there is at most one road between each pair of showplaces.</span></p></div><div class="output-specification"><p>Print the single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the maximum number of showplaces that Irina can visit during her journey from showplace <span class="tex-span">1</span> to showplace <span class="tex-span"><i>n</i></span> within time not exceeding <span class="tex-span"><i>T</i></span>, in the first line.</p><p>Print <span class="tex-span"><i>k</i></span> distinct integers in the second line&nbsp;— indices of showplaces that Irina will visit on her route, in the order of encountering them.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000,  1 ≤ <i>m</i> ≤ 5000,  1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of showplaces, the number of roads between them and the time of Irina's stay in Berlatov respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines describes roads in Berlatov. <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span">3</span> integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), meaning that there is a road starting from showplace <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and leading to showplace <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and Irina spends <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> time units to pass it. It is guaranteed that the roads do not form cyclic routes.</p><p><span class="tex-font-style-bf">It is guaranteed, that there is at most one road between each pair of showplaces.</span></p>

## Output

<p>Print the single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the maximum number of showplaces that Irina can visit during her journey from showplace <span class="tex-span">1</span> to showplace <span class="tex-span"><i>n</i></span> within time not exceeding <span class="tex-span"><i>T</i></span>, in the first line.</p><p>Print <span class="tex-span"><i>k</i></span> distinct integers in the second line&nbsp;— indices of showplaces that Irina will visit on her route, in the order of encountering them.</p><p>If there are multiple answers, print any of them.</p>





```input1
4 3 13
1 2 5
2 3 7
2 4 8

```




```input2
6 6 7
1 2 2
1 3 3
3 6 3
2 4 2
4 6 2
6 5 1

```




```input3
5 5 6
1 3 3
3 5 3
1 2 2
2 4 3
4 5 2

```




```output1
3
1 2 4 

```




```output2
4
1 2 4 6 

```




```output3
3
1 3 5 

```


