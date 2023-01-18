## Description

<div><p>Life is not easy for the perfectly common variable named Vasya. Wherever it goes, it is either assigned a value, or simply ignored, or is being used!</p><p>Vasya's life goes in states of a program. In each state, Vasya can either be used (for example, to calculate the value of another variable), or be assigned a value, or ignored. Between some states are directed (oriented) transitions.</p><p>A <span class="tex-font-style-it">path</span> is a sequence of states <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>x</i></sub></span>, where for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>x</i></span> exists a transition from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p><p>Vasya's value in state <span class="tex-span"><i>v</i></span> is interesting to the world, if exists path <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> such, that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>v</i></span> for some <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>k</i>)</span>, in state <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> Vasya gets assigned a value, in state <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span> Vasya is used and there is no state <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (except for <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>) where Vasya gets assigned a value.</p><p>Help Vasya, find the states in which Vasya's value is interesting to the world.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the numbers of states and transitions, correspondingly.</p><p>The second line contains space-separated <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> described actions performed upon Vasya in state <span class="tex-span"><i>i</i></span>: <span class="tex-span">0</span> represents ignoring, <span class="tex-span">1</span> — assigning a value, <span class="tex-span">2</span> — using.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain space-separated pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), each pair represents the transition from the state number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the state number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Between two states can be any number of transitions.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, separated by spaces or new lines. Number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> should equal <span class="tex-span">1</span>, if Vasya's value in state <span class="tex-span"><i>i</i></span> is interesting to the world and otherwise, it should equal <span class="tex-span">0</span>. The states are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order, in which they are described in the input.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the numbers of states and transitions, correspondingly.</p><p>The second line contains space-separated <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> described actions performed upon Vasya in state <span class="tex-span"><i>i</i></span>: <span class="tex-span">0</span> represents ignoring, <span class="tex-span">1</span> — assigning a value, <span class="tex-span">2</span> — using.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain space-separated pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), each pair represents the transition from the state number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the state number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Between two states can be any number of transitions.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, separated by spaces or new lines. Number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> should equal <span class="tex-span">1</span>, if Vasya's value in state <span class="tex-span"><i>i</i></span> is interesting to the world and otherwise, it should equal <span class="tex-span">0</span>. The states are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order, in which they are described in the input.</p>





```input1
4 3
1 0 0 2
1 2
2 3
3 4

```




```input2
3 1
1 0 2
1 3

```




```input3
3 1
2 0 1
1 3

```




```output1
1
1
1
1

```




```output2
1
0
1

```




```output3
0
0
0

```



## Note

<p>In the first sample the program states can be used to make the only path in which the value of Vasya interests the world, 1 <img align="middle" class="tex-formula" src="file://MRnzY3D4.png" style="max-width: 100.0%;max-height: 100.0%;"> 2 <img align="middle" class="tex-formula" src="file://DwkcMfhZ.png" style="max-width: 100.0%;max-height: 100.0%;"> 3 <img align="middle" class="tex-formula" src="file://Q7mNQ4wr.png" style="max-width: 100.0%;max-height: 100.0%;"> 4; it includes all the states, so in all of them Vasya's value is interesting to the world.</p><p>The second sample the only path in which Vasya's value is interesting to the world is , — 1 <img align="middle" class="tex-formula" src="file://1aUdv3E3.png" style="max-width: 100.0%;max-height: 100.0%;"> 3; state 2 is not included there.</p><p>In the third sample we cannot make from the states any path in which the value of Vasya would be interesting to the world, so the value of Vasya is never interesting to the world.</p>
