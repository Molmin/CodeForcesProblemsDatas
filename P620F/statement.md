## Description

<div><p>You are given an array with <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i></span> queries. Each query is described by two integers <span class="tex-span">(<i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>Let's define the function <img align="middle" class="tex-formula" src="file://ybTnXQtP.png" style="max-width: 100.0%;max-height: 100.0%;">. The function is defined for only <span class="tex-span"><i>u</i> ≤ <i>v</i></span>.</p><p>For each query print the maximal value of the function <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>)</span> over all <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>x</i>, <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>,  <i>a</i><sub class="lower-index"><i>x</i></sub> ≤ <i>a</i><sub class="lower-index"><i>y</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup>,  1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">3</sup></span>) — the size of the array and the number of the queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) – the parameters of the <span class="tex-span"><i>j</i></span>-th query.</p></div><div class="output-specification"><p>For each query print the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> on a separate line — the maximal value of the function <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>)</span> over all <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>x</i>, <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>,  <i>a</i><sub class="lower-index"><i>x</i></sub> ≤ <i>a</i><sub class="lower-index"><i>y</i></sub></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup>,  1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">3</sup></span>) — the size of the array and the number of the queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) – the parameters of the <span class="tex-span"><i>j</i></span>-th query.</p>

## Output

<p>For each query print the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> on a separate line — the maximal value of the function <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>)</span> over all <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>x</i>, <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>,  <i>a</i><sub class="lower-index"><i>x</i></sub> ≤ <i>a</i><sub class="lower-index"><i>y</i></sub></span>.</p>





```input1
6 3
1 2 3 4 5 6
1 6
2 5
3 4

```




```input2
1 1
1
1 1

```




```input3
6 20
10 21312 2314 214 1 322
1 1
1 2
1 3
1 4
1 5
1 6
2 2
2 3
2 4
2 5
2 6
3 4
3 5
3 6
4 4
4 5
4 6
5 5
5 6
6 6

```




```output1
7
7
7

```




```output2
1

```




```output3
10
21313
21313
21313
21313
21313
21312
21313
21313
21313
21313
2314
2315
2315
214
215
323
1
323
322

```


