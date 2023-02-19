## Description

<div><p>It's the turn of the year, so Bash wants to send presents to his friends. There are <span class="tex-span"><i>n</i></span> cities in the Himalayan region and they are connected by <span class="tex-span"><i>m</i></span> bidirectional roads. Bash is living in city <span class="tex-span"><i>s</i></span>. Bash has exactly one friend in each of the other cities. Since Bash wants to surprise his friends, he decides to send a Pikachu to each of them. <span class="tex-font-style-bf">Since there may be some cities which are not reachable from Bash's city, he only sends a Pikachu to those friends who live in a city reachable from his own city</span>. He also wants to send it to them as soon as possible.</p><p>He finds out the minimum time for each of his Pikachus to reach its destination city. Since he is a perfectionist, he informs all his friends with the time their gift will reach them. A Pikachu travels at a speed of <span class="tex-span">1</span> meters per second. His friends were excited to hear this and would be unhappy if their presents got delayed. Unfortunately Team Rocket is on the loose and they came to know of Bash's plan. They want to maximize the number of friends who are unhappy with Bash.</p><p>They do this by destroying exactly one of the other <span class="tex-span"><i>n</i> - 1</span> cities. This implies that <span class="tex-font-style-bf">the friend residing in that city dies, so he is unhappy as well</span>.</p><p>Note that <span class="tex-font-style-bf">if a city is destroyed, all the roads directly connected to the city are also destroyed and the Pikachu may be forced to take a longer alternate route</span>.</p><p><span class="tex-font-style-bf">Please also note that only friends that are waiting for a gift count as unhappy, even if they die.</span></p><p>Since Bash is already a legend, can you help Team Rocket this time and find out the maximum number of Bash's friends who can be made unhappy by destroying exactly one city.</p></div><div class="input-specification"><p>The first line contains three space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://TZsRBlHz.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of cities and the number of roads in the Himalayan region and the city Bash lives in.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) denoting that there exists a road between city <span class="tex-span"><i>u</i></span> and city <span class="tex-span"><i>v</i></span> of length <span class="tex-span"><i>w</i></span> meters.</p><p>It is guaranteed that no road connects a city to itself and there are no two roads that connect the same pair of cities.</p></div><div class="output-specification"><p>Print a single integer, the answer to the problem.</p></div>

## Input

<p>The first line contains three space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://TZsRBlHz.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of cities and the number of roads in the Himalayan region and the city Bash lives in.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) denoting that there exists a road between city <span class="tex-span"><i>u</i></span> and city <span class="tex-span"><i>v</i></span> of length <span class="tex-span"><i>w</i></span> meters.</p><p>It is guaranteed that no road connects a city to itself and there are no two roads that connect the same pair of cities.</p>

## Output

<p>Print a single integer, the answer to the problem.</p>





```input1
4 4 3
1 2 1
2 3 1
2 4 1
3 1 1

```




```input2
7 11 2
1 2 5
1 3 5
2 4 2
2 5 2
3 6 3
3 7 3
4 6 2
3 4 2
6 7 3
4 5 7
4 7 7

```




```output1
2

```




```output2
4

```



## Note

<p>In the first sample, on destroying the city <span class="tex-span">2</span>, the length of shortest distance between pairs of cities <span class="tex-span">(3, 2)</span> and <span class="tex-span">(3, 4)</span> will change. Hence the answer is <span class="tex-span">2</span>.</p>
