## Description

<div><p>Emuskald is a well-known illusionist. One of his trademark tricks involves a set of magical boxes. The essence of the trick is in packing the boxes inside other boxes.</p><p>From the top view each magical box looks like a square with side length equal to <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> (<span class="tex-span"><i>k</i></span> is an integer, <span class="tex-span"><i>k</i> ≥ 0</span>) units. A magical box <span class="tex-span"><i>v</i></span> can be put inside a magical box <span class="tex-span"><i>u</i></span>, if side length of <span class="tex-span"><i>v</i></span> is strictly less than the side length of <span class="tex-span"><i>u</i></span>. In particular, Emuskald can put 4 boxes of side length <span class="tex-span">2<sup class="upper-index"><i>k</i> - 1</sup></span> into one box of side length <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span>, or as in the following figure:</p><center> <img class="tex-graphics" src="file://dNShvVQ7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Emuskald is about to go on tour performing around the world, and needs to pack his magical boxes for the trip. He has decided that the best way to pack them would be inside another magical box, but magical boxes are quite expensive to make. Help him find the smallest magical box that can fit all his boxes.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of different sizes of boxes Emuskald has. Each of following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which means that Emuskald has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> boxes with side length <span class="tex-span">2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup></span>. It is guaranteed that all of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Output a single integer <span class="tex-span"><i>p</i></span>, such that the smallest magical box that can contain all of Emuskald’s boxes has side length <span class="tex-span">2<sup class="upper-index"><i>p</i></sup></span>.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of different sizes of boxes Emuskald has. Each of following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which means that Emuskald has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> boxes with side length <span class="tex-span">2<sup class="upper-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sup></span>. It is guaranteed that all of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Output a single integer <span class="tex-span"><i>p</i></span>, such that the smallest magical box that can contain all of Emuskald’s boxes has side length <span class="tex-span">2<sup class="upper-index"><i>p</i></sup></span>.</p>





```input1
2
0 3
1 5

```




```input2
1
0 4

```




```input3
2
1 10
2 2

```




```output1
3

```




```output2
1

```




```output3
3

```



## Note

<p><span class="tex-font-style-bf">Picture explanation</span>. If we have 3 boxes with side length 2 and 5 boxes with side length 1, then we can put all these boxes inside a box with side length 4, for example, as shown in the picture.</p><p>In the second test case, we can put all four small boxes into a box with side length 2.</p>
