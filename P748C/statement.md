## Description

<div><p>Santa Claus has Robot which lives on the infinite grid and can move <span class="tex-font-style-bf">along its lines</span>. He can also, having a sequence of <span class="tex-span"><i>m</i></span> points <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> with integer coordinates, do the following: denote its initial location by <span class="tex-span"><i>p</i><sub class="lower-index">0</sub></span>. First, the robot will move from <span class="tex-span"><i>p</i><sub class="lower-index">0</sub></span> to <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> along one of the shortest paths between them (please notice that since the robot moves only along the grid lines, there can be several shortest paths). Then, after it reaches <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, it'll move to <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, again, choosing one of the shortest ways, then to <span class="tex-span"><i>p</i><sub class="lower-index">3</sub></span>, and so on, until he has visited all points in the given order. Some of the points in the sequence may coincide, in that case Robot will visit that point several times according to the sequence order.</p><p>While Santa was away, someone gave a sequence of points to Robot. This sequence is now lost, but Robot saved the protocol of its unit movements. Please, find the minimum possible length of the sequence.</p></div><div class="input-specification"><p>The first line of input contains the only positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) which equals the number of unit segments the robot traveled. The second line contains the movements protocol, which consists of <span class="tex-span"><i>n</i></span> letters, each being equal either <span class="tex-font-style-tt">L</span>, or <span class="tex-font-style-tt">R</span>, or <span class="tex-font-style-tt">U</span>, or <span class="tex-font-style-tt">D</span>. <span class="tex-span"><i>k</i></span>-th letter stands for the direction which Robot traveled the <span class="tex-span"><i>k</i></span>-th unit segment in: <span class="tex-font-style-tt">L</span> means that it moved to the left, <span class="tex-font-style-tt">R</span>&nbsp;— to the right, <span class="tex-font-style-tt">U</span>&nbsp;— to the top and <span class="tex-font-style-tt">D</span>&nbsp;— to the bottom. Have a look at the illustrations for better explanation.</p></div><div class="output-specification"><p>The only line of input should contain the minimum possible length of the sequence.</p></div>

## Input

<p>The first line of input contains the only positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) which equals the number of unit segments the robot traveled. The second line contains the movements protocol, which consists of <span class="tex-span"><i>n</i></span> letters, each being equal either <span class="tex-font-style-tt">L</span>, or <span class="tex-font-style-tt">R</span>, or <span class="tex-font-style-tt">U</span>, or <span class="tex-font-style-tt">D</span>. <span class="tex-span"><i>k</i></span>-th letter stands for the direction which Robot traveled the <span class="tex-span"><i>k</i></span>-th unit segment in: <span class="tex-font-style-tt">L</span> means that it moved to the left, <span class="tex-font-style-tt">R</span>&nbsp;— to the right, <span class="tex-font-style-tt">U</span>&nbsp;— to the top and <span class="tex-font-style-tt">D</span>&nbsp;— to the bottom. Have a look at the illustrations for better explanation.</p>

## Output

<p>The only line of input should contain the minimum possible length of the sequence.</p>





```input1
4
RURD

```




```input2
6
RRULDD

```




```input3
26
RRRULURURUULULLLDLDDRDRDLD

```




```input4
3
RLL

```




```input5
4
LRLR

```




```output1
2

```




```output2
2

```




```output3
7

```




```output4
2

```




```output5
4

```



## Note

<p>The illustrations to the first three tests are given below.</p><p><img class="tex-graphics" src="file://Kb2OFkME.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://8ADDknhj.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://L9SBtl8g.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The last example illustrates that each point in the sequence should be counted as many times as it is presented in the sequence.</p>
