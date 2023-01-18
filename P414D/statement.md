## Description

<div><p>Mashmokh is playing a new game. In the beginning he has <span class="tex-span"><i>k</i></span> liters of water and <span class="tex-span"><i>p</i></span> coins. Additionally he has a rooted tree (an undirected connected acyclic graph) that consists of <span class="tex-span"><i>m</i></span> vertices. Each vertex of the tree contains a water tank that is empty in the beginning.</p><p>The game begins with the fact that Mashmokh chooses some (no more than <span class="tex-span"><i>k</i></span>) of these tanks (except the root) and pours into each of them exactly <span class="tex-span">1</span> liter of water. Then the following process is performed until there is no water remained in tanks.</p><ul> <li> The process consists of several steps. </li><li> At the beginning of each step Mashmokh opens doors of all tanks. Then Mashmokh closes doors of some tanks (he is not allowed to close door of tank in the root) for the duration of this move. Let's denote the number of liters in some tank with closed door as <span class="tex-span"><i>w</i></span>, Mashmokh pays <span class="tex-span"><i>w</i></span> coins for the closing of that tank during this move. </li><li> Let's denote by <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> as the list of vertices of the tree sorted (nondecreasing) by their depth. The vertices from this list should be considered one by one in the order. Firstly vertex <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> (which is the root itself) is emptied. Then for each vertex <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>i</i> &gt; 1)</span>, if its door is closed then skip the vertex else move all the water from the tank of vertex <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to the tank of its father (even if the tank of the father is closed). </li></ul><p>Suppose <span class="tex-span"><i>l</i></span> moves were made until the tree became empty. Let's denote the amount of water inside the tank of the root after the <span class="tex-span"><i>i</i></span>-th move by <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> then Mashmokh will win <span class="tex-span"><i>max</i>(<i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>l</i></sub>)</span> dollars. Mashmokh wanted to know what is the maximum amount of dollars he can win by playing the above game. He asked you to find this value for him.</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>m</i>, <i>k</i>, <i>p</i>&nbsp;(2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i>, <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </p><p>Each of the following <span class="tex-span"><i>m</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the edges of the tree.</p><p>Consider that the vertices of the tree are numbered from 1 to <span class="tex-span"><i>m</i></span>. The root of the tree has number 1.</p></div><div class="output-specification"><p>Output a single integer, the number Mashmokh asked you to find.</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>m</i>, <i>k</i>, <i>p</i>&nbsp;(2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i>, <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </p><p>Each of the following <span class="tex-span"><i>m</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the edges of the tree.</p><p>Consider that the vertices of the tree are numbered from 1 to <span class="tex-span"><i>m</i></span>. The root of the tree has number 1.</p>

## Output

<p>Output a single integer, the number Mashmokh asked you to find.</p>





```input1
10 2 1
1 2
1 3
3 4
3 5
2 6
6 8
6 7
9 8
8 10

```




```input2
5 1000 1000
1 2
1 3
3 4
3 5

```




```output1
2

```




```output2
4

```



## Note

<p>The tree in the first sample is shown on the picture below. The black, red, blue colors correspond to vertices with 0, 1, 2 liters of water.</p><center><img class="tex-graphics" src="file://if2Rd6O6.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>One way to achieve the maximum amount of money is to put 1 liter of water in each of vertices 3 and 4. The beginning state is shown on the picture below.</p><center><img class="tex-graphics" src="file://YON5NuEW.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Then in the first move Mashmokh will pay one token to close the door of the third vertex tank. The tree after the first move is shown on the picture below.</p><center><img class="tex-graphics" src="file://GGtWO0CZ.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>After the second move there are 2 liters of water in the root as shown on the picture below.</p><center><img class="tex-graphics" src="file://7Xzt9Opn.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
