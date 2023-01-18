## Description

<div><p>Little Mishka is a great traveller and she visited many countries. After thinking about where to travel this time, she chose XXX&nbsp;— beautiful, but little-known northern country.</p><p>Here are some interesting facts about XXX:</p><ol> <li> XXX consists of <span class="tex-span"><i>n</i></span> cities, <span class="tex-span"><i>k</i></span> of whose (just imagine!) are capital cities. </li><li> All of cities in the country are beautiful, but each is beautiful in its own way. Beauty value of <span class="tex-span"><i>i</i></span>-th city equals to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> All the cities are consecutively connected by the roads, including <span class="tex-span">1</span>-st and <span class="tex-span"><i>n</i></span>-th city, forming a cyclic route <span class="tex-span">1 — 2 — ... — <i>n</i> — 1</span>. Formally, for every <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span> there is a road between <span class="tex-span"><i>i</i></span>-th and <span class="tex-span"><i>i</i> + 1</span>-th city, and another one between <span class="tex-span">1</span>-st and <span class="tex-span"><i>n</i></span>-th city. </li><li> Each capital city is connected with each other city directly by the roads. Formally, if city <span class="tex-span"><i>x</i></span> is a capital city, then for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>,  <i>i</i> ≠ <i>x</i></span>, there is a road between cities <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>i</i></span>. </li><li> There is <span class="tex-font-style-bf">at most one</span> road between any two cities. </li><li> Price of passing a road directly depends on beauty values of cities it connects. Thus if there is a road between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, price of passing it equals <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>·<i>c</i><sub class="lower-index"><i>j</i></sub></span>.</li></ol><p>Mishka started to gather her things for a trip, but didn't still decide which route to follow and thus she asked you to help her determine summary price of passing <span class="tex-font-style-bf">each of the roads</span> in XXX. Formally, for every pair of cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> &lt; <i>b</i></span>), such that there is a road between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> you are to find sum of products <span class="tex-span"><i>c</i><sub class="lower-index"><i>a</i></sub>·<i>c</i><sub class="lower-index"><i>b</i></sub></span>. Will you help her?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of cities in XXX and the number of capital cities among them.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— beauty values of the cities.</p><p>The third line of the input contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of capital cities. Indices are given in ascending order.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— summary price of passing each of the roads in XXX.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of cities in XXX and the number of capital cities among them.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— beauty values of the cities.</p><p>The third line of the input contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of capital cities. Indices are given in ascending order.</p>

## Output

<p>Print the only integer&nbsp;— summary price of passing each of the roads in XXX.</p>





```input1
4 1
2 3 1 2
3

```




```input2
5 2
3 5 2 2 4
1 4

```




```output1
17
```




```output2
71
```



## Note

<p>This image describes first sample case:</p><p><img class="tex-graphics" src="file://FfOeY4yM.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>It is easy to see that summary price is equal to <span class="tex-span">17</span>.</p><p>This image describes second sample case:</p><p><img class="tex-graphics" src="file://r5xdhoo6.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>It is easy to see that summary price is equal to <span class="tex-span">71</span>.</p>
