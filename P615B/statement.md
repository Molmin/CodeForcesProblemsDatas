## Description

<div><p>This Christmas Santa gave Masha a magic picture and a pencil. The picture consists of <span class="tex-span"><i>n</i></span> points connected by <span class="tex-span"><i>m</i></span> segments (they might cross in any way, that doesn't matter). No two segments connect the same pair of points, and no segment connects the point to itself. Masha wants to color some segments in order paint a hedgehog. In Mashas mind every hedgehog consists of a tail and some spines. She wants to paint the tail that satisfies the following conditions: </p><ol> <li> Only segments already presented on the picture can be painted; </li><li> The tail should be continuous, i.e. consists of some sequence of points, such that every two neighbouring points are connected by a colored segment; </li><li> The numbers of points from the beginning of the tail to the end should strictly increase. </li></ol><p>Masha defines the length of the tail as the number of points in it. Also, she wants to paint some spines. To do so, Masha will paint all the segments, such that one of their ends is the <span class="tex-font-style-bf">endpoint</span> of the tail. Masha defines the beauty of a hedgehog as the length of the tail multiplied by the number of spines. Masha wants to color the most beautiful hedgehog. Help her calculate what result she may hope to get.</p><p>Note that according to Masha's definition of a hedgehog, one segment may simultaneously serve as a spine and a part of the tail (she is a little girl after all). Take a look at the picture for further clarifications.</p></div><div class="input-specification"><p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>(<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of points and the number segments on the picture respectively. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the numbers of points connected by corresponding segment. It's guaranteed that no two segments connect the same pair of points.</p></div><div class="output-specification"><p>Print the maximum possible value of the hedgehog's beauty.</p></div>

## Input

<p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>(<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of points and the number segments on the picture respectively. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each containing two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the numbers of points connected by corresponding segment. It's guaranteed that no two segments connect the same pair of points.</p>

## Output

<p>Print the maximum possible value of the hedgehog's beauty.</p>





```input1
8 6
4 5
3 5
2 5
1 2
2 8
6 7

```




```input2
4 6
1 2
1 3
1 4
2 3
2 4
3 4

```




```output1
9

```




```output2
12

```



## Note

<p>The picture below corresponds to the first sample. Segments that form the hedgehog are painted red. The tail consists of a sequence of points with numbers <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">5</span>. The following segments are spines: (<span class="tex-span">2</span>, <span class="tex-span">5</span>), (<span class="tex-span">3</span>, <span class="tex-span">5</span>) and (<span class="tex-span">4</span>, <span class="tex-span">5</span>). Therefore, the beauty of the hedgehog is equal to <span class="tex-span">3·3 = 9</span>.</p><p><img class="tex-graphics" src="file://bzw3HDQ1.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
