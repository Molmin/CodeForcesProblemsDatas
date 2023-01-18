## Description

<div><p><span class="tex-span"><i>n</i></span> ants are on a circle of length <span class="tex-span"><i>m</i></span>. An ant travels one unit of distance per one unit of time. Initially, the ant number <span class="tex-span"><i>i</i></span> is located at the position <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and is facing in the direction <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (which is either <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>). Positions are numbered in counterclockwise order starting from some point. Positions of the all ants are distinct.</p><p>All the ants move simultaneously, and whenever two ants touch, they will both switch their directions. Note that it is possible for an ant to move in some direction for a half of a unit of time and in opposite direction for another half of a unit of time.</p><p>Print the positions of the ants after <span class="tex-span"><i>t</i></span> time units.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of ants, the length of the circle and the number of time units.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and symbol <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is either <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>) — the position and the direction of the <span class="tex-span"><i>i</i></span>-th ant at the start. The directions <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span> corresponds to the clockwise and counterclockwise directions, respectively.</p><p>It is guaranteed that all positions <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> — the position of the <span class="tex-span"><i>j</i></span>-th ant after <span class="tex-span"><i>t</i></span> units of time. The ants are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of their appearing in input.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of ants, the length of the circle and the number of time units.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and symbol <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is either <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>) — the position and the direction of the <span class="tex-span"><i>i</i></span>-th ant at the start. The directions <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span> corresponds to the clockwise and counterclockwise directions, respectively.</p><p>It is guaranteed that all positions <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> — the position of the <span class="tex-span"><i>j</i></span>-th ant after <span class="tex-span"><i>t</i></span> units of time. The ants are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of their appearing in input.</p>





```input1
2 4 8
1 R
3 L

```




```input2
4 8 6
6 R
5 L
1 R
8 L

```




```input3
4 8 2
1 R
5 L
6 L
8 R

```




```output1
1 3

```




```output2
7 4 2 7

```




```output3
3 3 4 2

```


