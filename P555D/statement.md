## Description

<div><p>Andrewid the Android is a galaxy-famous detective. Now he is busy with a top secret case, the details of which are not subject to disclosure.</p><p>However, he needs help conducting one of the investigative experiment. There are <span class="tex-span"><i>n</i></span> pegs put on a plane, they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the coordinates of the <span class="tex-span"><i>i</i></span>-th of them are <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0)</span>. Then, we tie to the bottom of one of the pegs a weight on a tight rope of length <span class="tex-span"><i>l</i></span> (thus, its coordinates will be equal to <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>,  - <i>l</i>)</span>, where <span class="tex-span"><i>i</i></span> is the number of the used peg). Then the weight is pushed to the right, so that it starts to rotate counterclockwise. At the same time, if the weight during rotation touches some of the other pegs, it then begins to rotate around that peg. Suppose that each peg itself is very thin and does not affect the rope length while weight is rotating around it.</p><center> <img class="tex-graphics" src="file://ZRZZplCX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>More formally, if at some moment the segment of the rope contains one or more pegs in addition to the peg around which the weight is rotating, the weight will then rotate around the farthermost one of them on a shorter segment of a rope. In particular, if the segment of the rope touches some peg by its endpoint, it is considered that the weight starts to rotate around that peg on a segment of the rope of length <span class="tex-span">0</span>.</p><p>At some moment the weight will begin to rotate around some peg, without affecting the rest of the pegs. Andrewid interested in determining the number of this peg.</p><p>Andrewid prepared <span class="tex-span"><i>m</i></span> queries containing initial conditions for pushing the weight, help him to determine for each of them, around what peg the weight will eventually rotate.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of pegs and queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the pegs. It is guaranteed that the coordinates of all the pegs are distinct integers.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries of pushing the weight, each consists of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the starting peg and the length of the rope.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the number of the peg around which the weight will eventually rotate after the <span class="tex-span"><i>i</i></span>-th push.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of pegs and queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the pegs. It is guaranteed that the coordinates of all the pegs are distinct integers.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries of pushing the weight, each consists of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the starting peg and the length of the rope.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the number of the peg around which the weight will eventually rotate after the <span class="tex-span"><i>i</i></span>-th push.</p>





```input1
3 2
0 3 5
2 3
1 8

```




```input2
4 4
1 5 7 15
1 4
2 15
3 16
1 28

```




```output1
3
2

```




```output2
2
4
3
1

```



## Note

<p>Picture to the first sample test:</p><p><img class="tex-graphics" src="file://SJIWPgQo.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p>Picture to the second sample test:</p><p><img class="tex-graphics" src="file://z2WYQ7X6.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Note that in the last query weight starts to rotate around the peg 1 attached to a rope segment of length 0.</p>
