## Description

<div><p>You are given the following points with integer coordinates on the plane: <span class="tex-span"><i>M</i><sub class="lower-index">0</sub>, <i>A</i><sub class="lower-index">0</sub>, <i>A</i><sub class="lower-index">1</sub>, ..., <i>A</i><sub class="lower-index"><i>n</i> - 1</sub></span>, where <span class="tex-span"><i>n</i></span> is odd number. Now we define the following infinite sequence of points <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span>: <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i></sub></span> is symmetric to <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i> - 1</sub></span> according <img align="middle" class="tex-formula" src="file://VreKB21i.png" style="max-width: 100.0%;max-height: 100.0%;"> (for every natural number <span class="tex-span"><i>i</i></span>). Here point <span class="tex-span"><i>B</i></span> is symmetric to <span class="tex-span"><i>A</i></span> according <span class="tex-span"><i>M</i></span>, if <span class="tex-span"><i>M</i></span> is the center of the line segment <span class="tex-span"><i>AB</i></span>. Given index <span class="tex-span"><i>j</i></span> find the point <span class="tex-span"><i>M</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>On the first line you will be given an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), which will be odd, and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>j</i></span> is the index of the desired point. The next line contains two space separated integers, the coordinates of <span class="tex-span"><i>M</i><sub class="lower-index">0</sub></span>. After that <span class="tex-span"><i>n</i></span> lines follow, where the <span class="tex-span"><i>i</i></span>-th line contain the space separated integer coordinates of the point <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i> - 1</sub></span>. The absolute values of all input coordinates will not be greater then <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>On a single line output the coordinates of <span class="tex-span"><i>M</i><sub class="lower-index"><i>j</i></sub></span>, space separated.</p></div>

## Input

<p>On the first line you will be given an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), which will be odd, and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>j</i></span> is the index of the desired point. The next line contains two space separated integers, the coordinates of <span class="tex-span"><i>M</i><sub class="lower-index">0</sub></span>. After that <span class="tex-span"><i>n</i></span> lines follow, where the <span class="tex-span"><i>i</i></span>-th line contain the space separated integer coordinates of the point <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i> - 1</sub></span>. The absolute values of all input coordinates will not be greater then <span class="tex-span">1000</span>.</p>

## Output

<p>On a single line output the coordinates of <span class="tex-span"><i>M</i><sub class="lower-index"><i>j</i></sub></span>, space separated.</p>





```input1
3 4
0 0
1 1
2 3
-5 3

```




```input2
3 1
5 5
1000 1000
-1000 1000
3 100

```




```output1
14 0

```




```output2
1995 1995

```


