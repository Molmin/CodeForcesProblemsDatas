## Description

<div><p>Consider infinite grid of unit cells. Some of those cells are <span class="tex-font-style-it">planets</span>. </p><p><span class="tex-font-style-it">Meta-universe</span> <span class="tex-span"><i>M</i> = {<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub>}</span> is a set of planets. Suppose there is an infinite row or column with following two properties: 1) it doesn't contain any planet <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of meta-universe <span class="tex-span"><i>M</i></span> on it; 2) there are planets of <span class="tex-span"><i>M</i></span> located on both sides from this row or column. In this case we can turn the meta-universe <span class="tex-span"><i>M</i></span> into two non-empty meta-universes <span class="tex-span"><i>M</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>M</i><sub class="lower-index">2</sub></span> containing planets that are located on respective sides of this row or column. </p><p>A meta-universe which can't be split using operation above is called a <span class="tex-font-style-it">universe</span>. We perform such operations until all meta-universes turn to universes.</p><p>Given positions of the planets in the original meta-universe, find the number of universes that are result of described process. It can be proved that each universe is uniquely identified not depending from order of splitting.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of planets in the meta-universe.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th planet. All planets are located in different cells.</p></div><div class="output-specification"><p>Print the number of resulting universes.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of planets in the meta-universe.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th planet. All planets are located in different cells.</p>

## Output

<p>Print the number of resulting universes.</p>





```input1
5
0 0
0 2
2 0
2 1
2 2

```




```input2
8
0 0
1 0
0 2
0 3
3 0
3 1
2 3
3 3

```




```output1
3

```




```output2
1

```



## Note

<p>The following figure describes the first test case:</p><center> <img class="tex-graphics" src="file://TLYKPyYw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
