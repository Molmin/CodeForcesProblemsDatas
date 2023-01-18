## Description

<div><p>On a plane are <span class="tex-span"><i>n</i></span> points (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>) with integer coordinates between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">6</sup></span>. The distance between the two points with numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is said to be the following value: <img align="middle" class="tex-formula" src="file://3Pdgs8jx.png" style="max-width: 100.0%;max-height: 100.0%;"> (the distance calculated by such formula is called <span class="tex-font-style-it">Manhattan distance</span>).</p><p>We call a hamiltonian path to be some permutation <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. We say that the length of this path is value <img align="middle" class="tex-formula" src="file://rXs8hvQN.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Find some hamiltonian path with a length of no more than <span class="tex-span">25 × 10<sup class="upper-index">8</sup></span>. Note that you do not have to minimize the path length.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The <span class="tex-span"><i>i</i> + 1</span>-th line contains the coordinates of the <span class="tex-span"><i>i</i></span>-th point: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed that no two points coincide.</p></div><div class="output-specification"><p>Print the permutation of numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the sought Hamiltonian path. The permutation must meet the inequality <img align="middle" class="tex-formula" src="file://tgmHPXF9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>If there are multiple possible answers, print any of them.</p><p>It is guaranteed that the answer exists.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The <span class="tex-span"><i>i</i> + 1</span>-th line contains the coordinates of the <span class="tex-span"><i>i</i></span>-th point: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed that no two points coincide.</p>

## Output

<p>Print the permutation of numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the sought Hamiltonian path. The permutation must meet the inequality <img align="middle" class="tex-formula" src="file://tgmHPXF9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>If there are multiple possible answers, print any of them.</p><p>It is guaranteed that the answer exists.</p>





```input1
5
0 7
8 10
3 4
5 0
9 12

```




```output1
4 3 1 2 5 

```



## Note

<p>In the sample test the total distance is:</p><p><img align="middle" class="tex-formula" src="file://XAJdszZ5.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-span">(|5 - 3| + |0 - 4|) + (|3 - 0| + |4 - 7|) + (|0 - 8| + |7 - 10|) + (|8 - 9| + |10 - 12|) = 2 + 4 + 3 + 3 + 8 + 3 + 1 + 2 = 26</span></p>
