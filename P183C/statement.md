## Description

<div><p>You are given a <span class="tex-font-style-bf">directed</span> graph <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> arcs (<span class="tex-font-style-bf">multiple arcs and self-loops</span> are allowed). You have to paint each vertex of the graph into one of the <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> ≤ <i>n</i>)</span> colors in such way that for all arcs of the graph leading from a vertex <span class="tex-span"><i>u</i></span> to vertex <span class="tex-span"><i>v</i></span>, vertex <span class="tex-span"><i>v</i></span> is painted with the <span class="tex-font-style-it">next color</span> of the color used to paint vertex <span class="tex-span"><i>u</i></span>.</p><p>The colors are numbered cyclically <span class="tex-span">1</span> through <span class="tex-span"><i>k</i></span>. This means that for each color <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> &lt; <i>k</i>)</span> its next color is color <span class="tex-span"><i>i</i> + 1</span>. In addition, the next color of color <span class="tex-span"><i>k</i></span> is color <span class="tex-span">1</span>. Note, that if <span class="tex-span"><i>k</i> = 1</span>, then the next color for color <span class="tex-span">1</span> is again color <span class="tex-span">1</span>.</p><p>Your task is to find and print the largest possible value of <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> ≤ <i>n</i>)</span> such that it's possible to color <span class="tex-span"><i>G</i></span> as described above with <span class="tex-span"><i>k</i></span> colors. Note that you don't necessarily use all the <span class="tex-span"><i>k</i></span> colors (that is, for each color <span class="tex-span"><i>i</i></span> there does not necessarily exist a vertex that is colored with color <span class="tex-span"><i>i</i></span>).</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of vertices and the number of arcs of the given digraph, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each line will contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which means that the <span class="tex-span"><i>i</i></span>-th arc goes from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Multiple arcs and self-loops are allowed.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible number of the colors that can be used to paint the digraph (i.e. <span class="tex-span"><i>k</i></span>, as described in the problem statement). Note that the desired value of <span class="tex-span"><i>k</i></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of vertices and the number of arcs of the given digraph, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each line will contain two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which means that the <span class="tex-span"><i>i</i></span>-th arc goes from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Multiple arcs and self-loops are allowed.</p>

## Output

<p>Print a single integer — the maximum possible number of the colors that can be used to paint the digraph (i.e. <span class="tex-span"><i>k</i></span>, as described in the problem statement). Note that the desired value of <span class="tex-span"><i>k</i></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>.</p>





```input1
4 4
1 2
2 1
3 4
4 3

```




```input2
5 2
1 4
2 5

```




```input3
4 5
1 2
2 3
3 1
2 4
4 1

```




```input4
4 4
1 1
1 2
2 1
1 2

```




```output1
2

```




```output2
5

```




```output3
3

```




```output4
1

```



## Note

<p>For the first example, with <span class="tex-span"><i>k</i> = 2</span>, this picture depicts the two colors (arrows denote the next color of that color).</p><center> <img class="tex-graphics" src="file://lJHHbpwB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>With <span class="tex-span"><i>k</i> = 2</span> a possible way to paint the graph is as follows.</p><center> <img class="tex-graphics" src="file://k5e86f86.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It can be proven that no larger value for <span class="tex-span"><i>k</i></span> exists for this test case.</p><p>For the second example, here's the picture of the <span class="tex-span"><i>k</i> = 5</span> colors.</p><center> <img class="tex-graphics" src="file://BRSVd72W.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A possible coloring of the graph is:</p><center> <img class="tex-graphics" src="file://GzfXhA0j.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the third example, here's the picture of the <span class="tex-span"><i>k</i> = 3</span> colors.</p><center> <img class="tex-graphics" src="file://zdMctaMe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A possible coloring of the graph is:</p><center> <img class="tex-graphics" src="file://1lzs1TMh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
