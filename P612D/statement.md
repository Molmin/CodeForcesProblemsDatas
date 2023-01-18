## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> segments on the coordinate axis <span class="tex-font-style-tt">Ox</span> and the number <span class="tex-span"><i>k</i></span>. The point is <span class="tex-font-style-it">satisfied</span> if it belongs to at least <span class="tex-span"><i>k</i></span> segments. Find the smallest (by the number of segments) set of segments on the coordinate axis <span class="tex-font-style-tt">Ox</span> which contains all <span class="tex-font-style-it">satisfied</span> points and no others.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of segments and the value of <span class="tex-span"><i>k</i></span>.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) each — the endpoints of the <span class="tex-span"><i>i</i></span>-th segment. The segments can degenerate and intersect each other. The segments are given in arbitrary order.</p></div><div class="output-specification"><p>First line contains integer <span class="tex-span"><i>m</i></span> — the smallest number of segments.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub></span>) — the ends of <span class="tex-span"><i>j</i></span>-th segment in the answer. The segments should be listed in the order from left to right.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of segments and the value of <span class="tex-span"><i>k</i></span>.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) each — the endpoints of the <span class="tex-span"><i>i</i></span>-th segment. The segments can degenerate and intersect each other. The segments are given in arbitrary order.</p>

## Output

<p>First line contains integer <span class="tex-span"><i>m</i></span> — the smallest number of segments.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub></span>) — the ends of <span class="tex-span"><i>j</i></span>-th segment in the answer. The segments should be listed in the order from left to right.</p>





```input1
3 2
0 5
-3 2
3 8

```




```input2
3 2
0 5
-3 3
3 8

```




```output1
2
0 2
3 5

```




```output2
1
0 5

```


