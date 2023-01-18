## Description

<div><p>In some country live wizards. They love to build cities and roads.</p><p>The country used to have <span class="tex-span"><i>k</i></span> cities, the <span class="tex-span"><i>j</i></span>-th city (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>k</i></span>) was located at a point (<span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>). It was decided to create another <span class="tex-span"><i>n</i> - <i>k</i></span> cities. And the <span class="tex-span"><i>i</i></span>-th one (<span class="tex-span"><i>k</i> &lt; <i>i</i> ≤ <i>n</i></span>) was created at a point with coordinates (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>):</p><ul> <li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = (<i>a</i>·<i>x</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>b</i>)&nbsp;<i>mod</i>&nbsp;(10<sup class="upper-index">9</sup> + 9)</span> </li><li> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = (<i>c</i>·<i>y</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>d</i>)&nbsp;<i>mod</i>&nbsp;(10<sup class="upper-index">9</sup> + 9)</span> </li></ul><p>Here <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> are primes. Also, <span class="tex-span"><i>a</i> ≠ <i>c</i>, <i>b</i> ≠ <i>d</i></span>.</p><p>After the construction of all <span class="tex-span"><i>n</i></span> cities, the wizards have noticed something surprising. It turned out that for every two different cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span> holds.</p><p>The cities are built, it's time to build roads! It was decided to use the most difficult (and, of course, the most powerful) spell for the construction of roads. Using this spell creates a road between the towns of <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>y</i><sub class="lower-index"><i>u</i></sub></span> &gt; <span class="tex-span"><i>y</i><sub class="lower-index"><i>v</i></sub></span>) if and only if for any city <span class="tex-span"><i>w</i></span> which lies strictly inside the corner at the point <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (see below), there is a city <span class="tex-span"><i>s</i></span> that does not lie in the corner, which is located along the <span class="tex-span"><i>x</i></span>-coordinate strictly between <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>u</i></span> and simultaneously <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub> &gt; <i>y</i><sub class="lower-index"><i>v</i></sub></span>.</p><p>A <span class="tex-font-style-it">corner</span> on the points <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>(<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>), <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>(<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) (<span class="tex-span"><i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub></span>) is the set of points (<span class="tex-span"><i>x</i>, <i>y</i></span>), for which at least one of the two conditions is fulfilled: </p><ul> <li> <span class="tex-span"><i>min</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>) ≤ <i>x</i> ≤ <i>max</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>)</span> and <span class="tex-span"><i>y</i> ≥ <i>y</i><sub class="lower-index">1</sub></span> </li><li> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span> and <span class="tex-span">(<i>x</i> - <i>x</i><sub class="lower-index">2</sub>)·(<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>) ≥ 0</span> </li></ul><center> <img class="tex-graphics" src="file://UTtYDZEh.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The pictures showing two different corners </span> </center><p>In order to test the spell, the wizards will apply it to all the cities that lie on the <span class="tex-span"><i>x</i></span>-coordinate in the interval <span class="tex-span">[<i>L</i>, <i>R</i>]</span>. After the construction of roads the national government wants to choose the maximum number of pairs of cities connected by the road, so that no city occurs in two or more pairs. Your task is for each <span class="tex-span"><i>m</i></span> offered variants of values <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>R</i></span> to calculate the maximum number of such pairs after the construction of the roads. Please note that the cities that do not lie in the interval <span class="tex-span">[<i>L</i>, <i>R</i>]</span> on the <span class="tex-span"><i>x</i></span>-coordinate, do not affect the construction of roads in any way.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>k</i> ≤ 30</span>). Next <span class="tex-span"><i>k</i></span> lines contain coordinates of the cities' location points from the first to the <span class="tex-span"><i>k</i></span>-th one. The <span class="tex-span"><i>j</i></span>-th line contains space-separated pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> &lt; 10<sup class="upper-index">9</sup> + 9</span>) — coordinates of the <span class="tex-span"><i>j</i></span>-th city.</p><p>The next line contains space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> &lt; 10<sup class="upper-index">9</sup> + 9</span>). It is guaranteed that those numbers are prime and also that <span class="tex-span"><i>a</i> ≠ <i>c</i>, <i>b</i> ≠ <i>d</i></span>. </p><p>It's guaranteed, that for every two different cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span> holds.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of variants to build the roads. Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ <i>R</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup> + 9</span>) — the variants of choosing the cities to build the roads.</p></div><div class="output-specification"><p>For any pair of numbers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> print the answer to the problem on a single line. Print the answers for the pairs in the order, in which the pairs are given in the input data.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>k</i> ≤ 30</span>). Next <span class="tex-span"><i>k</i></span> lines contain coordinates of the cities' location points from the first to the <span class="tex-span"><i>k</i></span>-th one. The <span class="tex-span"><i>j</i></span>-th line contains space-separated pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> &lt; 10<sup class="upper-index">9</sup> + 9</span>) — coordinates of the <span class="tex-span"><i>j</i></span>-th city.</p><p>The next line contains space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> &lt; 10<sup class="upper-index">9</sup> + 9</span>). It is guaranteed that those numbers are prime and also that <span class="tex-span"><i>a</i> ≠ <i>c</i>, <i>b</i> ≠ <i>d</i></span>. </p><p>It's guaranteed, that for every two different cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span> holds.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of variants to build the roads. Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ <i>R</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup> + 9</span>) — the variants of choosing the cities to build the roads.</p>

## Output

<p>For any pair of numbers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> print the answer to the problem on a single line. Print the answers for the pairs in the order, in which the pairs are given in the input data.</p>





```input1
6 6
0 0
1 1
2 2
3 3
4 4
5 5
2 3 3 2
4
0 5
1 4
2 3
3 3

```




```input2
6 1
0 0
3 5 23917 11
4
0 1000000008
0 10
100 150
200 10000

```




```output1
3
2
1
0

```




```output2
2
1
0
1

```



## Note

<p>In the first sample the roads connect the cities in a chain in the order of increasing of <span class="tex-span"><i>x</i></span>. </p><p>In the second sample the remaining 5 cities will be located at points <span class="tex-span">(5, &nbsp;11);&nbsp;(20, &nbsp;263098);&nbsp;(65, &nbsp;292514823);&nbsp;(200, &nbsp;76958738);&nbsp;(605, &nbsp;622120197)</span>.</p>
