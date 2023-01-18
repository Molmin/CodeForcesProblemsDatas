## Description

<div><p>Kostya is a genial sculptor, he has an idea: to carve a marble sculpture in the shape of a sphere. Kostya has a friend Zahar who works at a career. Zahar knows about Kostya's idea and wants to present him a rectangular parallelepiped of marble from which he can carve the sphere. </p><p>Zahar has <span class="tex-span"><i>n</i></span> stones which are rectangular parallelepipeds. The edges sizes of the <span class="tex-span"><i>i</i></span>-th of them are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. He can take <span class="tex-font-style-bf">no more than two stones</span> and present them to Kostya. </p><p>If Zahar takes two stones, he should glue them together on one of the faces in order to get a new piece of rectangular parallelepiped of marble. Thus, it is possible to glue a pair of stones together if and only if two faces on which they are glued together match as rectangles. In such gluing it is allowed to rotate and flip the stones in any way. </p><p>Help Zahar choose such a present so that Kostya can carve a sphere of the maximum possible volume and present it to Zahar.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-span"><i>n</i></span> lines follow, in the <span class="tex-span"><i>i</i></span>-th of which there are three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the lengths of edges of the <span class="tex-span"><i>i</i></span>-th stone. Note, that two stones may have exactly the same sizes, but they still will be considered two different stones.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2</span>) the number of stones which Zahar has chosen. In the second line print <span class="tex-span"><i>k</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>&nbsp;— the numbers of stones which Zahar needs to choose. Consider that stones are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order as they are given in the input data.</p><p>You can print the stones in arbitrary order. If there are several answers print any of them. </p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-span"><i>n</i></span> lines follow, in the <span class="tex-span"><i>i</i></span>-th of which there are three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the lengths of edges of the <span class="tex-span"><i>i</i></span>-th stone. Note, that two stones may have exactly the same sizes, but they still will be considered two different stones.</p>

## Output

<p>In the first line print <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2</span>) the number of stones which Zahar has chosen. In the second line print <span class="tex-span"><i>k</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>&nbsp;— the numbers of stones which Zahar needs to choose. Consider that stones are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order as they are given in the input data.</p><p>You can print the stones in arbitrary order. If there are several answers print any of them. </p>





```input1
6
5 5 5
3 2 4
1 4 1
2 1 3
3 2 4
3 3 4

```




```input2
7
10 7 8
5 10 3
4 2 6
5 5 5
10 2 8
4 2 1
7 7 7

```




```output1
1
1

```




```output2
2
1 5

```



## Note

<p>In the first example we can connect the pairs of stones:</p><ul> <li> <span class="tex-span">2</span> and <span class="tex-span">4</span>, the size of the parallelepiped: <span class="tex-span">3 × 2 × 5</span>, the radius of the inscribed sphere <span class="tex-span">1</span> </li><li> <span class="tex-span">2</span> and <span class="tex-span">5</span>, the size of the parallelepiped: <span class="tex-span">3 × 2 × 8</span> or <span class="tex-span">6 × 2 × 4</span> or <span class="tex-span">3 × 4 × 4</span>, the radius of the inscribed sphere <span class="tex-span">1</span>, or <span class="tex-span">1</span>, or <span class="tex-span">1.5</span> respectively. </li><li> <span class="tex-span">2</span> and <span class="tex-span">6</span>, the size of the parallelepiped: <span class="tex-span">3 × 5 × 4</span>, the radius of the inscribed sphere <span class="tex-span">1.5</span> </li><li> <span class="tex-span">4</span> and <span class="tex-span">5</span>, the size of the parallelepiped: <span class="tex-span">3 × 2 × 5</span>, the radius of the inscribed sphere <span class="tex-span">1</span> </li><li> <span class="tex-span">5</span> and <span class="tex-span">6</span>, the size of the parallelepiped: <span class="tex-span">3 × 4 × 5</span>, the radius of the inscribed sphere <span class="tex-span">1.5</span> </li></ul><p>Or take only one stone:</p><ul> <li> <span class="tex-font-style-bf"><span class="tex-span">1</span> the size of the parallelepiped: <span class="tex-span">5 × 5 × 5</span>, the radius of the inscribed sphere <span class="tex-span">2.5</span></span> </li><li> <span class="tex-span">2</span> the size of the parallelepiped: <span class="tex-span">3 × 2 × 4</span>, the radius of the inscribed sphere <span class="tex-span">1</span> </li><li> <span class="tex-span">3</span> the size of the parallelepiped: <span class="tex-span">1 × 4 × 1</span>, the radius of the inscribed sphere <span class="tex-span">0.5</span> </li><li> <span class="tex-span">4</span> the size of the parallelepiped: <span class="tex-span">2 × 1 × 3</span>, the radius of the inscribed sphere <span class="tex-span">0.5</span> </li><li> <span class="tex-span">5</span> the size of the parallelepiped: <span class="tex-span">3 × 2 × 4</span>, the radius of the inscribed sphere <span class="tex-span">1</span> </li><li> <span class="tex-span">6</span> the size of the parallelepiped: <span class="tex-span">3 × 3 × 4</span>, the radius of the inscribed sphere <span class="tex-span">1.5</span> </li></ul><p>It is most profitable to take only the first stone. </p>
