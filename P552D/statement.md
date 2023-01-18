## Description

<div><p>Vanya got bored and he painted <span class="tex-span"><i>n</i></span> distinct points on the plane. After that he connected all the points pairwise and saw that as a result many triangles were formed with vertices in the painted points. He asks you to count the number of the formed triangles with the <span class="tex-font-style-bf">non-zero</span> area.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of the points painted on the plane. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that no two given points coincide.</p></div><div class="output-specification"><p>In the first line print an integer — the number of triangles with the non-zero area among the painted points.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of the points painted on the plane. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that no two given points coincide.</p>

## Output

<p>In the first line print an integer — the number of triangles with the non-zero area among the painted points.</p>





```input1
4
0 0
1 1
2 0
2 2

```




```input2
3
0 0
1 1
2 0

```




```input3
1
1 1

```




```output1
3

```




```output2
1

```




```output3
0

```



## Note

<p>Note to the first sample test. There are <span class="tex-span">3</span> triangles formed: <span class="tex-span">(0, 0) - (1, 1) - (2, 0)</span>; <span class="tex-span">(0, 0) - (2, 2) - (2, 0)</span>; <span class="tex-span">(1, 1) - (2, 2) - (2, 0)</span>.</p><p>Note to the second sample test. There is <span class="tex-span">1</span> triangle formed: <span class="tex-span">(0, 0) - (1, 1) - (2, 0)</span>.</p><p>Note to the third sample test. A single point doesn't form a single triangle.</p>
