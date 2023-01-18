## Description

<div><p>Everybody knows that we have been living in the Matrix for a long time. And in the new seventh Matrix the world is ruled by beavers.</p><p>So let's take beaver Neo. Neo has so-called "deja vu" outbursts when he gets visions of events in some places he's been at or is going to be at. Let's examine the phenomenon in more detail.</p><p>We can say that Neo's city is represented by a directed graph, consisting of <span class="tex-span"><i>n</i></span> shops and <span class="tex-span"><i>m</i></span> streets that connect the shops. No two streets connect the same pair of shops (besides, there can't be one street from A to B and one street from B to A). No street connects a shop with itself. As Neo passes some streets, he gets visions. No matter how many times he passes street <span class="tex-span"><i>k</i></span>, every time he will get the same visions in the same order. A vision is a sequence of shops.</p><p>We know that Neo is going to get really shocked if he passes the way from some shop <span class="tex-span"><i>a</i></span> to some shop <span class="tex-span"><i>b</i></span>, possible coinciding with <span class="tex-span"><i>a</i></span>, such that the list of visited shops in the real life and in the visions coincide.</p><p>Suggest beaver Neo such path of non-zero length. Or maybe you can even count the number of such paths modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>?..</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of shops and the number of streets, correspondingly, <span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <img align="middle" class="tex-formula" src="file://yubMhqzV.png" style="max-width: 100.0%;max-height: 100.0%;">. Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the streets in the following format: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> ... <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are indices of shops connected by a street, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> is the number of visions on the way from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> describe the visions: the numbers of the shops Neo saw. Note that the order of the visions matters.</p><p>It is guaranteed that the total number of visions on all streets doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><ul> <li> to get 50 points, you need to find any (not necessarily simple) path of length at most <span class="tex-span">2·<i>n</i></span>, that meets the attributes described above (subproblem E1); </li><li> to get 50 more points, you need to count for each length from <span class="tex-span">1</span> to <span class="tex-span">2·<i>n</i></span> the number of paths that have the attribute described above (subproblem E2). </li></ul></div><div class="output-specification"><p>Subproblem E1. In the first line print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 2·<i>n</i>)</span> — the numbers of shops on Neo's path. In the next line print <span class="tex-span"><i>k</i></span> integers — the number of shops in the order Neo passes them. If the graph doesn't have such paths or the length of the shortest path includes more than <span class="tex-span">2·<i>n</i></span> shops, print on a single line <span class="tex-span">0</span>.</p><p>Subproblem E2. Print <span class="tex-span">2·<i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line must contain a single integer — the number of required paths of length <span class="tex-span"><i>i</i></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of shops and the number of streets, correspondingly, <span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <img align="middle" class="tex-formula" src="file://yubMhqzV.png" style="max-width: 100.0%;max-height: 100.0%;">. Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the streets in the following format: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> ... <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are indices of shops connected by a street, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> is the number of visions on the way from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> describe the visions: the numbers of the shops Neo saw. Note that the order of the visions matters.</p><p>It is guaranteed that the total number of visions on all streets doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><ul> <li> to get 50 points, you need to find any (not necessarily simple) path of length at most <span class="tex-span">2·<i>n</i></span>, that meets the attributes described above (subproblem E1); </li><li> to get 50 more points, you need to count for each length from <span class="tex-span">1</span> to <span class="tex-span">2·<i>n</i></span> the number of paths that have the attribute described above (subproblem E2). </li></ul>

## Output

<p>Subproblem E1. In the first line print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 2·<i>n</i>)</span> — the numbers of shops on Neo's path. In the next line print <span class="tex-span"><i>k</i></span> integers — the number of shops in the order Neo passes them. If the graph doesn't have such paths or the length of the shortest path includes more than <span class="tex-span">2·<i>n</i></span> shops, print on a single line <span class="tex-span">0</span>.</p><p>Subproblem E2. Print <span class="tex-span">2·<i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line must contain a single integer — the number of required paths of length <span class="tex-span"><i>i</i></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
6 6
1 2 2 1 2
2 3 1 3
3 4 2 4 5
4 5 0
5 3 1 3
6 1 1 6

```




```input2
6 6
1 2 2 1 2
2 3 1 3
3 4 2 4 5
4 5 0
5 3 1 3
6 1 1 6

```




```output1
4
6 1 2 3

```




```output2
1
2
1
1
2
1
1
2
1
1
2
1
```



## Note

<p>The input in both samples are the same. The first sample contains the answer to the first subproblem, the second sample contains the answer to the second subproblem.</p>
