## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> segments on a line. There are no ends of some segments that coincide. For each segment find the number of segments it contains.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of segments on a line.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the left and the right ends of the <span class="tex-span"><i>i</i></span>-th segment. It is guaranteed that there are no ends of some segments that coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>j</i></span>-th of them should contain the only integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the number of segments contained in the <span class="tex-span"><i>j</i></span>-th segment.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of segments on a line.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the left and the right ends of the <span class="tex-span"><i>i</i></span>-th segment. It is guaranteed that there are no ends of some segments that coincide.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>j</i></span>-th of them should contain the only integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> — the number of segments contained in the <span class="tex-span"><i>j</i></span>-th segment.</p>





```input1
4
1 8
2 3
4 7
5 6

```




```input2
3
3 4
1 5
2 6

```




```output1
3
0
1
0

```




```output2
0
1
1

```


