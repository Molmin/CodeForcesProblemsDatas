## Description

<div><p>Mishka received a gift of multicolored pencils for his birthday! Unfortunately he lives in a monochrome world, where everything is of the same color and only saturation differs. This pack can be represented as a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> integer numbers — saturation of the color of each pencil. Now Mishka wants to put all the mess in the pack in order. He has an infinite number of empty boxes to do this. He would like to fill some boxes in such a way that:</p><ul> <li> Each pencil belongs to <span class="tex-font-style-bf">exactly</span> one box; </li><li> Each non-empty box has at least <span class="tex-span"><i>k</i></span> pencils in it; </li><li> If pencils <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> belong to the same box, then <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>j</i></sub>| ≤ <i>d</i></span>, where <span class="tex-span">|<i>x</i>|</span> means absolute value of <span class="tex-span"><i>x</i></span>. Note that the opposite is optional, there can be pencils <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>j</i></sub>| ≤ <i>d</i></span> and they belong to different boxes. </li></ul><p>Help Mishka to determine if it's possible to distribute all the pencils into boxes. Print "<span class="tex-font-style-tt">YES</span>" if there exists such a distribution. Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of pencils, minimal size of any non-empty box and maximal difference in saturation between any pair of pencils in the same box, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — saturation of color of each pencil.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if it's possible to distribute all the pencils into boxes and satisfy all the conditions. Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of pencils, minimal size of any non-empty box and maximal difference in saturation between any pair of pencils in the same box, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — saturation of color of each pencil.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if it's possible to distribute all the pencils into boxes and satisfy all the conditions. Otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
6 3 10
7 2 7 7 4 2

```




```input2
6 2 3
4 5 3 13 4 10

```




```input3
3 2 5
10 16 22

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first example it is possible to distribute pencils into <span class="tex-span">2</span> boxes with <span class="tex-span">3</span> pencils in each with any distribution. And you also can put all the pencils into the same box, difference of any pair in it won't exceed <span class="tex-span">10</span>.</p><p>In the second example you can split pencils of saturations <span class="tex-span">[4, 5, 3, 4]</span> into <span class="tex-span">2</span> boxes of size <span class="tex-span">2</span> and put the remaining ones into another box.</p>
