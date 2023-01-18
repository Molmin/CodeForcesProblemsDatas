## Description

<div><p>There is a straight line colored in white. <span class="tex-span"><i>n</i></span> black segments are added on it one by one.</p><p>After each segment is added, determine the number of connected components of black segments (i.&nbsp;e. the number of black segments in the union of the black segments). </p><p>In particular, if one segment ends in a point <span class="tex-span"><i>x</i></span>, and another segment starts in the point <span class="tex-span"><i>x</i></span>, these two segments belong to the same connected component.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of segments.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the left and the right ends of the <span class="tex-span"><i>i</i></span>-th segment. The segments are listed in the order they are added on the white line.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers — the number of connected components of black segments after each segment is added. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of segments.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the left and the right ends of the <span class="tex-span"><i>i</i></span>-th segment. The segments are listed in the order they are added on the white line.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers — the number of connected components of black segments after each segment is added. </p>





```input1
3
1 3
4 5
2 4

```




```input2
9
10 20
50 60
30 40
70 80
90 100
60 70
10 40
40 50
80 90

```




```output1
1 2 1 

```




```output2
1 2 3 4 5 4 3 2 1 

```



## Note

<p>In the first example there are two components after the addition of the first two segments, because these segments do not intersect. The third added segment intersects the left segment and touches the right segment at the point <span class="tex-span">4</span> (these segments belong to the same component, according to the statements). Thus the number of connected components of black segments is equal to <span class="tex-span">1</span> after that.</p>
