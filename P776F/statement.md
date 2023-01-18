## Description

<div><p>Sherlock met Moriarty for a final battle of wits. He gave him a regular <span class="tex-span"><i>n</i></span> sided convex polygon. In addition to it, he gave him certain diagonals to form regions on the polygon. It was guaranteed that the diagonals did not intersect in interior points.</p><p>He took each of the region and calculated its importance value. Importance value for a region formed by vertices <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>x</i></sub></span> of the polygon will be given by <span class="tex-span">2<sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup> + 2<sup class="upper-index"><i>a</i><sub class="lower-index">2</sub></sup> + ... + 2<sup class="upper-index"><i>a</i><sub class="lower-index"><i>x</i></sub></sup></span>. Then, he sorted these regions on the basis of their importance value in ascending order. After that he assigned each region an index from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, where <span class="tex-span"><i>k</i></span> is the number of regions, and index of region is its position in the sorted array calculated above.</p><p>He wants Moriarty to color the regions using not more than <span class="tex-span">20</span> colors, such that two regions have same color only if all the simple paths between these two regions have at least one region with color value less than the color value assigned to these regions. Simple path between two regions <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>h</i></span> is a sequence of regions <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ... <i>r</i><sub class="lower-index"><i>t</i></sub></span> such that <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> = <i>f</i></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>t</i></sub> = <i>h</i></span>, for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>t</i></span> regions <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i> + 1</sub></span> share an edge, and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>j</i></sub></span> if and only if <span class="tex-span"><i>i</i> = <i>j</i></span>.</p><p>Moriarty couldn't answer and asks Sherlock to solve it himself. Help Sherlock in doing so.</p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> - 3</span>), the number of vertices in the polygon and the number of diagonals added.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>), describing a diagonal between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. It is guaranteed that the diagonals are correct, i.&nbsp;e. <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> don't coincide and are not neighboring. It is guaranteed that the diagonals do not intersect.</p></div><div class="output-specification"><p>Let the number of regions be <span class="tex-span"><i>k</i></span>.</p><p>Output <span class="tex-span"><i>k</i></span> space-separated integers, each between <span class="tex-span">1</span> and <span class="tex-span">20</span>, representing the colors of the regions in the order of increasing importance.</p><p>If there are multiple answers, print any of them. It can be shown that at least one answer exists.</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> - 3</span>), the number of vertices in the polygon and the number of diagonals added.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>), describing a diagonal between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. It is guaranteed that the diagonals are correct, i.&nbsp;e. <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> don't coincide and are not neighboring. It is guaranteed that the diagonals do not intersect.</p>

## Output

<p>Let the number of regions be <span class="tex-span"><i>k</i></span>.</p><p>Output <span class="tex-span"><i>k</i></span> space-separated integers, each between <span class="tex-span">1</span> and <span class="tex-span">20</span>, representing the colors of the regions in the order of increasing importance.</p><p>If there are multiple answers, print any of them. It can be shown that at least one answer exists.</p>





```input1
4 1
1 3

```




```input2
6 3
1 3
1 4
1 5

```




```output1
1 2

```




```output2
2 1 2 3

```



## Note

<p>In 2nd input, regions formed in order after sorting will be <span class="tex-span">(1, 2, 3)</span>, <span class="tex-span">(1, 3, 4)</span>, <span class="tex-span">(1, 4, 5)</span>, <span class="tex-span">(1, 5, 6)</span>, i.e, region <span class="tex-span">(1, 2, 3)</span> is first region followed by region <span class="tex-span">(1, 3, 4)</span> and so on.</p><p>So, we can color regions <span class="tex-span">1</span> and <span class="tex-span">3</span> with same color, as region number <span class="tex-span">2</span> is on the path from <span class="tex-span">1</span> to <span class="tex-span">3</span> and it has color <span class="tex-span">1</span> which is less than color of <span class="tex-span">1</span> and <span class="tex-span">3</span>, i.e., color number <span class="tex-span">2</span>.</p>
