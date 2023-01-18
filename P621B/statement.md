## Description

<div><p>Today, Wet Shark is given <span class="tex-span"><i>n</i></span> bishops on a <span class="tex-span">1000</span> by <span class="tex-span">1000</span> grid. Both rows and columns of the grid are numbered from <span class="tex-span">1</span> to <span class="tex-span">1000</span>. Rows are numbered from top to bottom, while columns are numbered from left to right.</p><p>Wet Shark thinks that two bishops attack each other if they share the same diagonal. Note, that this is the only criteria, so two bishops may attack each other (according to Wet Shark) even if there is another bishop located between them. Now Wet Shark wants to count the number of pairs of bishops that attack each other.</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of bishops.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains two space separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the number of row and the number of column where <span class="tex-span"><i>i</i></span>-th bishop is positioned. It's guaranteed that no two bishops share the same position.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the number of pairs of bishops which attack each other. </p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of bishops.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains two space separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the number of row and the number of column where <span class="tex-span"><i>i</i></span>-th bishop is positioned. It's guaranteed that no two bishops share the same position.</p>

## Output

<p>Output one integer&nbsp;— the number of pairs of bishops which attack each other. </p>





```input1
5
1 1
1 5
3 3
5 1
5 5

```




```input2
3
1 1
2 3
3 5

```




```output1
6

```




```output2
0

```



## Note

<p>In the first sample following pairs of bishops attack each other: <span class="tex-span">(1, 3)</span>, <span class="tex-span">(1, 5)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(3, 4)</span> and <span class="tex-span">(3, 5)</span>. Pairs <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 4)</span>, <span class="tex-span">(2, 5)</span> and <span class="tex-span">(4, 5)</span> do not attack each other because they do not share the same diagonal.</p>
