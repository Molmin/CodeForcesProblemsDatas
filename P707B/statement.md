## Description

<div><p>Masha wants to open her own bakery and bake muffins in one of the <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There are <span class="tex-span"><i>m</i></span> bidirectional roads, each of whose connects some pair of cities.</p><p>To bake muffins in her bakery, Masha needs to establish flour supply from some storage. There are only <span class="tex-span"><i>k</i></span> storages, located in different cities numbered <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Unforunately the law of the country Masha lives in prohibits opening bakery in any of the cities which has storage located in it. She can open it only in one of another <span class="tex-span"><i>n</i> - <i>k</i></span> cities, and, of course, flour delivery should be paid&nbsp;— for every kilometer of path between storage and bakery Masha should pay <span class="tex-span">1</span> ruble.</p><p>Formally, Masha will pay <span class="tex-span"><i>x</i></span> roubles, if she will open the bakery in some city <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i></span> for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>) and choose a storage in some city <span class="tex-span"><i>s</i></span> (<span class="tex-span"><i>s</i> = <i>a</i><sub class="lower-index"><i>j</i></sub></span> for some <span class="tex-span">1 ≤ <i>j</i> ≤ <i>k</i></span>) and <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>s</i></span> are connected by some path of roads of summary length <span class="tex-span"><i>x</i></span> (if there are more than one path, Masha is able to choose which of them should be used).</p><p>Masha is very thrifty and rational. She is interested in a city, where she can open her bakery (and choose one of <span class="tex-span"><i>k</i></span> storages and one of the paths between city with bakery and city with storage) and pay minimum possible amount of rubles for flour delivery. Please help Masha find this amount.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of cities in country Masha lives in, the number of roads between them and the number of flour storages respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. Each of them contains three integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>) meaning that there is a road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> of length of <span class="tex-span"><i>l</i></span> kilometers .</p><p>If <span class="tex-span"><i>k</i> &gt; 0</span>, then the last line of the input contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of cities having flour storage located in. If <span class="tex-span"><i>k</i> = 0</span> then this line <span class="tex-font-style-bf">is not presented in the input</span>.</p></div><div class="output-specification"><p>Print the minimum possible amount of rubles Masha should pay for flour delivery in the only line.</p><p>If the bakery can not be opened (while satisfying conditions) in any of the <span class="tex-span"><i>n</i></span> cities, print <span class="tex-span"> - 1</span> in the only line.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of cities in country Masha lives in, the number of roads between them and the number of flour storages respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. Each of them contains three integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>) meaning that there is a road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> of length of <span class="tex-span"><i>l</i></span> kilometers .</p><p>If <span class="tex-span"><i>k</i> &gt; 0</span>, then the last line of the input contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of cities having flour storage located in. If <span class="tex-span"><i>k</i> = 0</span> then this line <span class="tex-font-style-bf">is not presented in the input</span>.</p>

## Output

<p>Print the minimum possible amount of rubles Masha should pay for flour delivery in the only line.</p><p>If the bakery can not be opened (while satisfying conditions) in any of the <span class="tex-span"><i>n</i></span> cities, print <span class="tex-span"> - 1</span> in the only line.</p>





```input1
5 4 2
1 2 5
1 2 3
2 3 4
1 4 10
1 5

```




```input2
3 1 1
1 2 3
3

```




```output1
3
```




```output2
-1
```



## Note

<center><img class="tex-graphics" src="file://ZStGnZwp.png" style="max-width: 100.0%;max-height: 100.0%;"><p>Image illustrates the first sample case. Cities with storage located in and the road representing the answer are darkened. </p></center>
