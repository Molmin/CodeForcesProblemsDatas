## Description

<div><p>A flowerbed has many flowers and two fountains.</p><p>You can adjust the water pressure and set any values <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>(<i>r</i><sub class="lower-index">1</sub> ≥ 0)</span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub>(<i>r</i><sub class="lower-index">2</sub> ≥ 0)</span>, giving the distances at which the water is spread from the first and second fountain respectively. You have to set such <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> that all the flowers are watered, that is, for each flower, the distance between the flower and the first fountain doesn't exceed <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, or the distance to the second fountain doesn't exceed <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>. It's OK if some flowers are watered by both fountains.</p><p>You need to decrease the amount of water you need, that is set such <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> that all the flowers are watered and the <span class="tex-span"><i>r</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> + <i>r</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup></span> is minimum possible. Find this minimum value.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the number of flowers, the coordinates of the first and the second fountain.</p><p>Next follow <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th flower.</p><p>It is guaranteed that all <span class="tex-span"><i>n</i> + 2</span> points in the input are distinct.</p></div><div class="output-specification"><p>Print the minimum possible value <span class="tex-span"><i>r</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> + <i>r</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup></span>. Note, that in this problem optimal answer is always integer.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the number of flowers, the coordinates of the first and the second fountain.</p><p>Next follow <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th flower.</p><p>It is guaranteed that all <span class="tex-span"><i>n</i> + 2</span> points in the input are distinct.</p>

## Output

<p>Print the minimum possible value <span class="tex-span"><i>r</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> + <i>r</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup></span>. Note, that in this problem optimal answer is always integer.</p>





```input1
2 -1 0 5 3
0 2
5 2

```




```input2
4 0 0 5 0
9 4
8 3
-1 0
1 4

```




```output1
6

```




```output2
33

```



## Note

<p>The first sample is (<span class="tex-span"><i>r</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> = 5</span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup> = 1</span>): <img class="tex-graphics" src="file://te754xxS.png" style="max-width: 100.0%;max-height: 100.0%;"> The second sample is (<span class="tex-span"><i>r</i><sub class="lower-index">1</sub><sup class="upper-index">2</sup> = 1</span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub><sup class="upper-index">2</sup> = 32</span>): <img class="tex-graphics" src="file://3tVvD59A.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
