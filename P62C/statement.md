## Description

<div><p>In Medieval times existed the tradition of burning witches at steaks together with their pets, black cats. By the end of the 15-th century the population of black cats ceased to exist. The difficulty of the situation led to creating the EIC - the Emergency Inquisitory Commission.</p><p>The resolution #666 says that a white cat is considered black when and only when the perimeter of its black spots exceeds the acceptable norm. But what does the acceptable norm equal to? Every inquisitor will choose it himself depending on the situation. And your task is to find the perimeter of black spots on the cat's fur.</p><p>The very same resolution says that the cat's fur is a white square with the length of <span class="tex-span">10<sup class="upper-index">5</sup></span>. During the measurement of spots it is customary to put the lower left corner of the fur into the origin of axes <span class="tex-span">(0;0)</span> and the upper right one — to the point with coordinates <span class="tex-span">(10<sup class="upper-index">5</sup>;10<sup class="upper-index">5</sup>)</span>. The cats' spots are nondegenerate triangles. The spots can intersect and overlap with each other, but it is guaranteed that each pair of the triangular spots' sides have no more than one common point.</p><p>We'll regard the perimeter in this problem as the total length of the boarders where a cat's fur changes color.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>). It is the number of spots on the cat's fur. The <span class="tex-span"><i>i</i></span>-th of the last <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span">6</span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3<i>i</i></sub></span>. They are the coordinates of the <span class="tex-span"><i>i</i></span>-th triangular spot <span class="tex-span">(0 &lt; <i>x</i><sub class="lower-index"><i>ji</i></sub>, <i>y</i><sub class="lower-index"><i>ji</i></sub> &lt; 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>Print a single number, the answer to the problem, perimeter of the union of triangles. Your answer should differ from the correct one in no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>). It is the number of spots on the cat's fur. The <span class="tex-span"><i>i</i></span>-th of the last <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span">6</span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3<i>i</i></sub></span>. They are the coordinates of the <span class="tex-span"><i>i</i></span>-th triangular spot <span class="tex-span">(0 &lt; <i>x</i><sub class="lower-index"><i>ji</i></sub>, <i>y</i><sub class="lower-index"><i>ji</i></sub> &lt; 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>Print a single number, the answer to the problem, perimeter of the union of triangles. Your answer should differ from the correct one in no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1
1 1 2 1 1 2

```




```input2
3
3 3 10 3 3 10
1 1 9 4 5 6
2 2 11 7 6 11

```




```output1
3.4142135624

```




```output2
37.7044021497

```


