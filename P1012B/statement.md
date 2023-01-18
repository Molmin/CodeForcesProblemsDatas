## Description

<div><p>Innopolis University scientists continue to investigate the periodic table. There are <span class="tex-span"><i>n</i>·<i>m</i></span> known elements and they form a periodic table: a rectangle with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each element can be described by its coordinates <span class="tex-span">(<i>r</i>, <i>c</i>)</span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>) in the table.</p><p>Recently scientists discovered that for every four different elements in this table that form a rectangle with sides parallel to the sides of the table, if they have samples of three of the four elements, they can produce a sample of the fourth element using nuclear fusion. So if we have elements in positions <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, where <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> ≠ <i>r</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> ≠ <i>c</i><sub class="lower-index">2</sub></span>, then we can produce element <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>.</p><center> <img class="tex-graphics" src="file://2Q7pPbIp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Samples used in fusion are not wasted and can be used again in future fusions. Newly crafted elements also can be used in future fusions.</p><p>Innopolis University scientists already have samples of <span class="tex-span"><i>q</i></span> elements. They want to obtain samples of all <span class="tex-span"><i>n</i>·<i>m</i></span> elements. To achieve that, they will purchase some samples from other laboratories and then produce all remaining elements using an arbitrary number of nuclear fusions in some order. Help them to find the minimal number of elements they need to purchase.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>; <span class="tex-span">0 ≤ <i>q</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 200 000)</span>), the chemical table dimensions and the number of elements scientists already have.</p><p>The following <span class="tex-span"><i>q</i></span> lines contain two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), each describes an element that scientists already have. All elements in the input are different.</p></div><div class="output-specification"><p>Print the minimal number of elements to be purchased.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>; <span class="tex-span">0 ≤ <i>q</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 200 000)</span>), the chemical table dimensions and the number of elements scientists already have.</p><p>The following <span class="tex-span"><i>q</i></span> lines contain two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), each describes an element that scientists already have. All elements in the input are different.</p>

## Output

<p>Print the minimal number of elements to be purchased.</p>





```input1
2 2 3
1 2
2 2
2 1

```




```input2
1 5 3
1 3
1 1
1 5

```




```input3
4 3 6
1 2
1 3
2 2
2 3
3 1
3 3

```




```output1
0

```




```output2
2

```




```output3
1

```



## Note

<p>For each example you have a picture which illustrates it.</p><p>The first picture for each example describes the initial set of element samples available. Black crosses represent elements available in the lab initially.</p><p>The second picture describes how remaining samples can be obtained. Red dashed circles denote elements that should be purchased from other labs (the optimal solution should minimize the number of red circles). Blue dashed circles are elements that can be produced with nuclear fusion. They are numbered in order in which they can be produced.</p><p><span class="tex-font-style-bf">Test 1</span></p><p>We can use nuclear fusion and get the element from three other samples, so we don't need to purchase anything.</p><center> <img class="tex-graphics" src="file://vQRXovfa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">Test 2</span></p><p>We cannot use any nuclear fusion at all as there is only one row, so we have to purchase all missing elements.</p><center> <img class="tex-graphics" src="file://lGcPctRh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">Test 3</span></p><p>There are several possible solutions. One of them is illustrated below.</p><p>Note that after purchasing one element marked as red it's still not possible to immidiately produce the middle element in the bottom row (marked as 4). So we produce the element in the left-top corner first (marked as 1), and then use it in future fusions.</p><center> <img class="tex-graphics" src="file://f3WenY8z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
