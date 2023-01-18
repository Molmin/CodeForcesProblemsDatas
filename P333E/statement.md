## Description

<div><p>Many schoolchildren look for a job for the summer, and one day, when Gerald was still a schoolboy, he also decided to work in the summer. But as Gerald was quite an unusual schoolboy, he found quite unusual work. A certain Company agreed to pay him a certain sum of money if he draws them three identical circles on a plane. The circles must not interfere with each other (but they may touch each other). He can choose the centers of the circles only from the <span class="tex-span"><i>n</i></span> options granted by the Company. He is free to choose the radius of the circles himself (all three radiuses must be equal), but please note that the larger the radius is, the more he gets paid. </p><p>Help Gerald earn as much as possible.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> — the number of centers (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>). The following <span class="tex-span"><i>n</i></span> lines each contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of potential circle centers, provided by the Company.</p><p>All given points are distinct.</p></div><div class="output-specification"><p>Print a single real number — maximum possible radius of circles. The answer will be accepted if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> — the number of centers (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>). The following <span class="tex-span"><i>n</i></span> lines each contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of potential circle centers, provided by the Company.</p><p>All given points are distinct.</p>

## Output

<p>Print a single real number — maximum possible radius of circles. The answer will be accepted if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
0 1
1 0
1 1

```




```input2
7
2 -3
-2 -3
3 0
-3 -1
1 -2
2 -2
-1 0

```




```output1
0.50000000000000000000

```




```output2
1.58113883008418980000

```


