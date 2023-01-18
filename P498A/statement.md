## Description

<div><p>Crazy Town is a plane on which there are <span class="tex-span"><i>n</i></span> infinite line roads. Each road is defined by the equation <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> + <i>c</i><sub class="lower-index"><i>i</i></sub> = 0</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are not both equal to the zero. The roads divide the plane into connected regions, possibly of infinite space. Let's call each such region a block. We define an intersection as the point where at least two different roads intersect.</p><p>Your home is located in one of the blocks. Today you need to get to the University, also located in some block. In one step you can move from one block to another, if the length of their common border is nonzero (in particular, this means that if the blocks are adjacent to one intersection, but have no shared nonzero boundary segment, then it are not allowed to move from one to another one in one step).</p><p>Determine what is the minimum number of steps you have to perform to get to the block containing the university. It is guaranteed that neither your home nor the university is located on the road.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of your home.</p><p>The second line contains two integers separated by a space <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of the university you are studying at.</p><p>The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the number of roads in the city. The following <span class="tex-span"><i>n</i></span> lines contain 3 space-separated integers (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| + |<i>b</i><sub class="lower-index"><i>i</i></sub>| &gt; 0</span>) — the coefficients of the line <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> + <i>c</i><sub class="lower-index"><i>i</i></sub> = 0</span>, defining the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that no two roads are the same. In addition, neither your home nor the university lie on the road (i.e. they do not belong to any one of the lines).</p></div><div class="output-specification"><p>Output the answer to the problem.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of your home.</p><p>The second line contains two integers separated by a space <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of the university you are studying at.</p><p>The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the number of roads in the city. The following <span class="tex-span"><i>n</i></span> lines contain 3 space-separated integers (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| + |<i>b</i><sub class="lower-index"><i>i</i></sub>| &gt; 0</span>) — the coefficients of the line <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> + <i>c</i><sub class="lower-index"><i>i</i></sub> = 0</span>, defining the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that no two roads are the same. In addition, neither your home nor the university lie on the road (i.e. they do not belong to any one of the lines).</p>

## Output

<p>Output the answer to the problem.</p>





```input1
1 1
-1 -1
2
0 1 0
1 0 0

```




```input2
1 1
-1 -1
3
1 0 0
0 1 0
1 1 -3

```




```output1
2

```




```output2
2

```



## Note

<p>Pictures to the samples are presented below (A is the point representing the house; B is the point representing the university, different blocks are filled with different colors):</p><center> <img class="tex-graphics" src="file://txXstQDl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://f0VNq4gy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
