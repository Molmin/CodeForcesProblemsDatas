## Description

<div><p>Many computer strategy games require building cities, recruiting army, conquering tribes, collecting resources. Sometimes it leads to interesting problems. </p><p>Let's suppose that your task is to build a square city. The world map uses the Cartesian coordinates. The sides of the city should be parallel to coordinate axes. The map contains mines with valuable resources, located at some points with integer coordinates. The sizes of mines are relatively small, i.e. they can be treated as points. The city should be built in such a way that all the mines are inside or on the border of the city square. </p><p>Building a city takes large amount of money depending on the size of the city, so you have to build the city with the minimum area. Given the positions of the mines find the minimum possible area of the city.</p></div><div class="input-specification"><p>The first line of the input contains number <span class="tex-span"><i>n</i></span>&nbsp;— the number of mines on the map (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the coordinates of the corresponding mine (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). All points are pairwise distinct.</p></div><div class="output-specification"><p>Print the minimum area of the city that can cover all the mines with valuable resources.</p></div>

## Input

<p>The first line of the input contains number <span class="tex-span"><i>n</i></span>&nbsp;— the number of mines on the map (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the coordinates of the corresponding mine (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). All points are pairwise distinct.</p>

## Output

<p>Print the minimum area of the city that can cover all the mines with valuable resources.</p>





```input1
2
0 0
2 2

```




```input2
2
0 0
0 3

```




```output1
4

```




```output2
9

```


