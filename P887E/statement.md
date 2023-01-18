## Description

<div><p>Masha's little brother draw two points on a sheet of paper. After that, he draws some circles and gave the sheet to his sister. </p><p>Masha has just returned from geometry lesson so she instantly noticed some interesting facts about brother's drawing.</p><p>At first, the line going through two points, that brother drew, doesn't intersect or touch any circle.</p><p>Also, no two circles intersect or touch, and there is no pair of circles such that one circle is located inside another.</p><p>Moreover, for each circle, Masha drew a square of the minimal area with sides parallel axis such that this circle is located inside the square and noticed that there is no two squares intersect or touch and there is no pair of squares such that one square is located inside other.</p><p>Now Masha wants to draw circle of minimal possible radius such that it goes through two points that brother drew and doesn't intersect any other circle, but other circles can touch Masha's circle and can be located inside it.</p><p><span class="tex-font-style-bf">It's guaranteed, that answer won't exceed <span class="tex-span">10<sup class="upper-index">12</sup></span>. It should be held for hacks as well.</span></p></div><div class="input-specification"><p>First line contains four integers <span class="tex-span"><i>x</i>1</span>, <span class="tex-span"><i>y</i>1</span>, <span class="tex-span"><i>x</i>2</span>, <span class="tex-span"><i>y</i>2</span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i>1, <i>y</i>1, <i>x</i>2, <i>y</i>2 ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— coordinates of points that brother drew. First point has coordinates (<span class="tex-span"><i>x</i>1</span>, <span class="tex-span"><i>y</i>1</span>) and second point has coordinates (<span class="tex-span"><i>x</i>2</span>, <span class="tex-span"><i>y</i>2</span>). These two points are different.</p><p>The second line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of circles that brother drew.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains descriptions of circles. Each line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) describing circle with center (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>) and radius <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Output smallest real number, that it's possible to draw a circle with such radius through given points in such a way that it doesn't intersect other circles.</p><p>The output is considered correct if it has a relative or absolute error of at most <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>First line contains four integers <span class="tex-span"><i>x</i>1</span>, <span class="tex-span"><i>y</i>1</span>, <span class="tex-span"><i>x</i>2</span>, <span class="tex-span"><i>y</i>2</span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i>1, <i>y</i>1, <i>x</i>2, <i>y</i>2 ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— coordinates of points that brother drew. First point has coordinates (<span class="tex-span"><i>x</i>1</span>, <span class="tex-span"><i>y</i>1</span>) and second point has coordinates (<span class="tex-span"><i>x</i>2</span>, <span class="tex-span"><i>y</i>2</span>). These two points are different.</p><p>The second line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of circles that brother drew.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains descriptions of circles. Each line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) describing circle with center (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>) and radius <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Output smallest real number, that it's possible to draw a circle with such radius through given points in such a way that it doesn't intersect other circles.</p><p>The output is considered correct if it has a relative or absolute error of at most <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
2 4 7 13
3
3 0 1
12 4 2
-4 14 2

```




```input2
-2 3 10 -10
2
7 0 3
-5 -5 2

```




```output1
5.1478150705
```




```output2
9.1481831923
```



## Note

<p><img class="tex-graphics" src="file://Ru6nnw0X.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://vMjHbzNt.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
