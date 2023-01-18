## Description

<div><center> <img class="tex-graphics" src="file://YPT4odLz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As some of you know, cubism is a trend in art, where the problem of constructing volumetrical shape on a plane with a combination of three-dimensional geometric shapes comes to the fore. </p><p>A famous sculptor Cicasso, whose self-portrait you can contemplate, hates cubism. He is more impressed by the idea to transmit two-dimensional objects through three-dimensional objects by using his magnificent sculptures. And his new project is connected with this. Cicasso wants to make a coat for the haters of anticubism. To do this, he wants to create a sculpture depicting a well-known geometric primitive — <span class="tex-font-style-it">convex polygon</span>.</p><p>Cicasso prepared for this a few blanks, which are rods with integer lengths, and now he wants to bring them together. The <span class="tex-span"><i>i</i></span>-th rod is a segment of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The sculptor plans to make a convex polygon with a nonzero area, using <span class="tex-font-style-it">all</span> rods he has as its sides. Each rod should be used as a side to its full length. It is forbidden to cut, break or bend rods. However, two sides may form a straight angle <img align="middle" class="tex-formula" src="file://AVUibOux.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Cicasso knows that it is impossible to make a convex polygon with a nonzero area out of the rods with the lengths which he had chosen. Cicasso does not want to leave the unused rods, so the sculptor decides to make another rod-blank with an integer length so that his problem is solvable. Of course, he wants to make it as short as possible, because the materials are expensive, and it is improper deed to spend money for nothing. </p><p>Help sculptor! </p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — a number of rod-blanks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — lengths of rods, which Cicasso already has. It is guaranteed that it is impossible to make a polygon with <span class="tex-span"><i>n</i></span> vertices and nonzero area using the rods Cicasso already has.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>z</i></span> — the minimum length of the rod, so that after adding it it can be possible to construct convex polygon with <span class="tex-span">(<i>n</i> + 1)</span> vertices and nonzero area from all of the rods.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — a number of rod-blanks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — lengths of rods, which Cicasso already has. It is guaranteed that it is impossible to make a polygon with <span class="tex-span"><i>n</i></span> vertices and nonzero area using the rods Cicasso already has.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>z</i></span> — the minimum length of the rod, so that after adding it it can be possible to construct convex polygon with <span class="tex-span">(<i>n</i> + 1)</span> vertices and nonzero area from all of the rods.</p>





```input1
3
1 2 1

```




```input2
5
20 4 3 2 1

```




```output1
1

```




```output2
11

```



## Note

<p>In the first example triangle with sides <span class="tex-span">{1 + 1 = 2, 2, 1}</span> can be formed from a set of lengths <span class="tex-span">{1, 1, 1, 2}</span>. </p><p>In the second example you can make a triangle with lengths <span class="tex-span">{20, 11, 4 + 3 + 2 + 1 = 10}</span>. </p>
