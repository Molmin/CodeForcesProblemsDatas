## Description

<div><p>Polycarpus has <span class="tex-span"><i>n</i></span> markers and <span class="tex-span"><i>m</i></span> marker caps. Each marker is described by two numbers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the color and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the diameter. Correspondingly, each cap is described by two numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is the color and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is the diameter. Cap <span class="tex-span">(<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>)</span> can close marker <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> only if their diameters match, that is, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub></span>. Besides, a marker is considered to be <span class="tex-font-style-it">beautifully closed</span>, if the cap color and the marker color match, that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Find the way to close the maximum number of markers. If there are several such ways, then choose the one that has the maximum number of <span class="tex-font-style-it">beautifully closed</span> markers.</p></div><div class="input-specification"><p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of markers and the number of caps, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the markers. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the <span class="tex-span"><i>i</i></span>-th marker's color and diameter, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the caps. The <span class="tex-span"><i>j</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 1000</span>) — the color and diameter of the <span class="tex-span"><i>j</i></span>-th cap, correspondingly.</p></div><div class="output-specification"><p>Print two space-separated integers <span class="tex-span"><i>u</i>, <i>v</i></span>, where <span class="tex-span"><i>u</i></span> is the number of closed markers and <span class="tex-span"><i>v</i></span> is the number of <span class="tex-font-style-it">beautifully closed</span> markers in the sought optimal way. Remember that you have to find the way to close the maximum number of markers, and if there are several such ways, you should choose the one where the number of <span class="tex-font-style-it">beautifully closed</span> markers is maximum.</p></div>

## Input

<p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of markers and the number of caps, correspondingly. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the markers. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the <span class="tex-span"><i>i</i></span>-th marker's color and diameter, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the caps. The <span class="tex-span"><i>j</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 1000</span>) — the color and diameter of the <span class="tex-span"><i>j</i></span>-th cap, correspondingly.</p>

## Output

<p>Print two space-separated integers <span class="tex-span"><i>u</i>, <i>v</i></span>, where <span class="tex-span"><i>u</i></span> is the number of closed markers and <span class="tex-span"><i>v</i></span> is the number of <span class="tex-font-style-it">beautifully closed</span> markers in the sought optimal way. Remember that you have to find the way to close the maximum number of markers, and if there are several such ways, you should choose the one where the number of <span class="tex-font-style-it">beautifully closed</span> markers is maximum.</p>





```input1
3 4
1 2
3 4
2 4
5 4
2 4
1 1
1 2

```




```input2
2 2
1 2
2 1
3 4
5 1

```




```output1
3 2

```




```output2
1 0

```



## Note

<p>In the first test sample the first marker should be closed by the fourth cap, the second marker should be closed by the first cap and the third marker should be closed by the second cap. Thus, three markers will be closed, and two of them will be <span class="tex-font-style-it">beautifully closed</span> — the first and the third markers.</p>
