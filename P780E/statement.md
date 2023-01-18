## Description

<div><p>The evil Bumbershoot corporation produces clones for gruesome experiments in a vast underground lab. On one occasion, the corp cloned a boy Andryusha who was smarter than his comrades. Immediately Andryusha understood that something fishy was going on there. He rallied fellow clones to go on a feud against the evil corp, and they set out to find an exit from the lab. The corp had to reduce to destroy the lab complex.</p><p>The lab can be pictured as a connected graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. <span class="tex-span"><i>k</i></span> clones of Andryusha start looking for an exit in some of the vertices. Each clone can traverse any edge once per second. Any number of clones are allowed to be at any vertex simultaneously. Each clone is allowed to stop looking at any time moment, but he must look at his starting vertex at least. The exit can be located at any vertex of the lab, hence each vertex must be visited by at least one clone.</p><p>Each clone can visit at most <img align="middle" class="tex-formula" src="file://OqvLbAw6.png" style="max-width: 100.0%;max-height: 100.0%;"> vertices before the lab explodes.</p><p>Your task is to choose starting vertices and searching routes for the clones. Each route can have at most <img align="middle" class="tex-formula" src="file://quOyMkdp.png" style="max-width: 100.0%;max-height: 100.0%;"> vertices.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of vertices and edges in the lab, and the number of clones.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by the respective edge. The graph is allowed to have self-loops and multiple edges.</p><p>The graph is guaranteed to be connected.</p></div><div class="output-specification"><p>You should print <span class="tex-span"><i>k</i></span> lines. <span class="tex-span"><i>i</i></span>-th of these lines must start with an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://DviogXjC.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices visited by <span class="tex-span"><i>i</i></span>-th clone, followed by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> integers&nbsp;— indices of vertices visited by this clone in the order of visiting. You have to print each vertex every time it is visited, regardless if it was visited earlier or not.</p><p>It is guaranteed that a valid answer exists.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of vertices and edges in the lab, and the number of clones.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by the respective edge. The graph is allowed to have self-loops and multiple edges.</p><p>The graph is guaranteed to be connected.</p>

## Output

<p>You should print <span class="tex-span"><i>k</i></span> lines. <span class="tex-span"><i>i</i></span>-th of these lines must start with an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://DviogXjC.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices visited by <span class="tex-span"><i>i</i></span>-th clone, followed by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> integers&nbsp;— indices of vertices visited by this clone in the order of visiting. You have to print each vertex every time it is visited, regardless if it was visited earlier or not.</p><p>It is guaranteed that a valid answer exists.</p>





```input1
3 2 1
2 1
3 1

```




```input2
5 4 2
1 2
1 3
1 4
1 5

```




```output1
3 2 1 3

```




```output2
3 2 1 3
3 4 1 5
```



## Note

<p>In the first sample case there is only one clone who may visit vertices in order (2, 1, 3), which fits the constraint of 6 vertices per clone.</p><p>In the second sample case the two clones can visited vertices in order (2, 1, 3) and (4, 1, 5), which fits the constraint of 5 vertices per clone.</p>
