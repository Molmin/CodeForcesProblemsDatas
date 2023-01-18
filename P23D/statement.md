## Description

<div><p>You're given the centers of three equal sides of a strictly convex tetragon. Your task is to restore the initial tetragon.</p></div><div class="input-specification"><p>The first input line contains one number <span class="tex-span"><i>T</i></span> — amount of tests (<span class="tex-span">1 ≤ <i>T</i> ≤ 5·10<sup class="upper-index">4</sup></span>). Each of the following <span class="tex-span"><i>T</i></span> lines contains numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span> — coordinates of different points that are the centers of three equal sides (non-negative integer numbers, not exceeding 10).</p></div><div class="output-specification"><p>For each test output two lines. If the required tetragon exists, output in the first line <span class="tex-font-style-tt">YES</span>, in the second line — four pairs of numbers — coordinates of the polygon's vertices in clockwise or counter-clockwise order. Don't forget, please, that the tetragon should be strictly convex, i.e. no 3 of its points lie on one line. Output numbers with 9 characters after a decimal point.</p><p>If the required tetragon doen't exist, output <span class="tex-font-style-tt">NO</span> in the first line, and leave the second line empty.</p></div>

## Input

<p>The first input line contains one number <span class="tex-span"><i>T</i></span> — amount of tests (<span class="tex-span">1 ≤ <i>T</i> ≤ 5·10<sup class="upper-index">4</sup></span>). Each of the following <span class="tex-span"><i>T</i></span> lines contains numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span> — coordinates of different points that are the centers of three equal sides (non-negative integer numbers, not exceeding 10).</p>

## Output

<p>For each test output two lines. If the required tetragon exists, output in the first line <span class="tex-font-style-tt">YES</span>, in the second line — four pairs of numbers — coordinates of the polygon's vertices in clockwise or counter-clockwise order. Don't forget, please, that the tetragon should be strictly convex, i.e. no 3 of its points lie on one line. Output numbers with 9 characters after a decimal point.</p><p>If the required tetragon doen't exist, output <span class="tex-font-style-tt">NO</span> in the first line, and leave the second line empty.</p>





```input1
3
1 1 2 2 3 3
0 1 1 0 2 2
9 3 7 9 9 8

```




```output1
NO

YES
3.5 1.5 0.5 2.5 -0.5 -0.5 2.5 0.5
NO


```


