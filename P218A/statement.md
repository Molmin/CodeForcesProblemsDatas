## Description

<div><p>Little Bolek has found a picture with <span class="tex-span"><i>n</i></span> mountain peaks painted on it. The <span class="tex-span"><i>n</i></span> painted peaks are represented by a non-closed polyline, consisting of <span class="tex-span">2<i>n</i></span> segments. The segments go through <span class="tex-span">2<i>n</i> + 1</span> points with coordinates <span class="tex-span">(1, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(2, <i>y</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">...</span>, <span class="tex-span">(2<i>n</i> + 1, <i>y</i><sub class="lower-index">2<i>n</i> + 1</sub>)</span>, with the <span class="tex-span"><i>i</i></span>-th segment connecting the point <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and the point <span class="tex-span">(<i>i</i> + 1, <i>y</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>. For any even <span class="tex-span"><i>i</i></span> <span class="tex-span">(2 ≤ <i>i</i> ≤ 2<i>n</i>)</span> the following condition holds: <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> &gt; <i>y</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </p><p>We shall call a vertex of a polyline with an even <span class="tex-span"><i>x</i></span> coordinate a <span class="tex-font-style-it">mountain peak</span>.</p><center> <img class="tex-graphics" src="file://g2T94vuH.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The figure to the left shows the initial picture, the figure to the right shows what the picture looks like after Bolek's actions. The affected peaks are marked red, <span class="tex-span"><i>k</i></span> = 2. </span> </center><p>Bolek fancied a little mischief. He chose exactly <span class="tex-span"><i>k</i></span> mountain peaks, rubbed out the segments that went through those peaks and increased each peak's height by one (that is, he increased the <span class="tex-span"><i>y</i></span> coordinate of the corresponding points). Then he painted the missing segments to get a new picture of mountain peaks. Let us denote the points through which the new polyline passes on Bolek's new picture as <span class="tex-span">(1, <i>r</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(2, <i>r</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">...</span>, <span class="tex-span">(2<i>n</i> + 1, <i>r</i><sub class="lower-index">2<i>n</i> + 1</sub>)</span>.</p><p>Given Bolek's final picture, restore the initial one.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span>. The next line contains <span class="tex-span">2<i>n</i> + 1</span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index">2<i>n</i> + 1</sub></span> <span class="tex-span">(0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the <span class="tex-span"><i>y</i></span> coordinates of the polyline vertices on Bolek's picture.</p><p>It is guaranteed that we can obtain the given picture after performing the described actions on some picture of mountain peaks.</p></div><div class="output-specification"><p>Print <span class="tex-span">2<i>n</i> + 1</span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index">2<i>n</i> + 1</sub></span> — the <span class="tex-span"><i>y</i></span> coordinates of the vertices of the polyline on the initial picture. If there are multiple answers, output any one of them.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span>. The next line contains <span class="tex-span">2<i>n</i> + 1</span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index">2<i>n</i> + 1</sub></span> <span class="tex-span">(0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the <span class="tex-span"><i>y</i></span> coordinates of the polyline vertices on Bolek's picture.</p><p>It is guaranteed that we can obtain the given picture after performing the described actions on some picture of mountain peaks.</p>

## Output

<p>Print <span class="tex-span">2<i>n</i> + 1</span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index">2<i>n</i> + 1</sub></span> — the <span class="tex-span"><i>y</i></span> coordinates of the vertices of the polyline on the initial picture. If there are multiple answers, output any one of them.</p>





```input1
3 2
0 5 3 5 1 5 2

```




```input2
1 1
0 2 0

```




```output1
0 5 3 4 1 4 2 

```




```output2
0 1 0 

```


