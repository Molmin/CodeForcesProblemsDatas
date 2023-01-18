## Description

<div><p>One day, Okazaki Tomoya has bought a tree for Furukawa Nagisa's birthday. The tree is so strange that every node of the tree has a value. The value of the <span class="tex-span"><i>i</i></span>-th node is <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Now Furukawa Nagisa and Okazaki Tomoya want to play a game on the tree.</p><p>Let <span class="tex-span">(<i>s</i>, <i>e</i>)</span> be the path from node <span class="tex-span"><i>s</i></span> to node <span class="tex-span"><i>e</i></span>, we can write down the sequence of the values of nodes on path <span class="tex-span">(<i>s</i>, <i>e</i>)</span>, and denote this sequence as <span class="tex-span"><i>S</i>(<i>s</i>, <i>e</i>)</span>. We define the value of the sequence <span class="tex-span"><i>G</i>(<i>S</i>(<i>s</i>, <i>e</i>))</span> as follows. Suppose that the sequence is <span class="tex-span"><i>z</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">1</sub>...<i>z</i><sub class="lower-index"><i>l</i> - 1</sub></span>, where <span class="tex-span"><i>l</i></span> is the length of the sequence. We define <span class="tex-span"><i>G</i>(<i>S</i>(<i>s</i>, <i>e</i>)) = <i>z</i><sub class="lower-index">0</sub> × <i>k</i><sup class="upper-index">0</sup> + <i>z</i><sub class="lower-index">1</sub> × <i>k</i><sup class="upper-index">1</sup> + ... + <i>z</i><sub class="lower-index"><i>l</i> - 1</sub> × <i>k</i><sup class="upper-index"><i>l</i> - 1</sup></span>. If the path <span class="tex-span">(<i>s</i>, <i>e</i>)</span> satisfies <img align="middle" class="tex-formula" src="file://LDhaUw8l.png" style="max-width: 100.0%;max-height: 100.0%;">, then the path <span class="tex-span">(<i>s</i>, <i>e</i>)</span> belongs to Furukawa Nagisa, otherwise it belongs to Okazaki Tomoya.</p><p>Calculating who has more paths is too easy, so they want to play something more difficult. Furukawa Nagisa thinks that if paths <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>)</span> and <span class="tex-span">(<i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>)</span> belong to her, then path <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">3</sub>)</span> belongs to her as well. Also, she thinks that if paths <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>)</span> and <span class="tex-span">(<i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>)</span> belong to Okazaki Tomoya, then path <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">3</sub>)</span> belongs to Okazaki Tomoya as well. But in fact, this conclusion isn't always right. So now Furukawa Nagisa wants to know how many triplets <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>)</span> are correct for the conclusion, and this is your task.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> &lt; <i>y</i>;&nbsp;0 ≤ <i>x</i> &lt; <i>y</i>)</span> — <span class="tex-span"><i>n</i></span> being the number of nodes on the tree. It is guaranteed that <span class="tex-span"><i>y</i></span> is a prime number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i>)</span>.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, each line contains two integers, denoting an edge of the tree. The nodes of the tree are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Output a single integer — the number of triplets that are correct for Furukawa Nagisa's conclusion.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> &lt; <i>y</i>;&nbsp;0 ≤ <i>x</i> &lt; <i>y</i>)</span> — <span class="tex-span"><i>n</i></span> being the number of nodes on the tree. It is guaranteed that <span class="tex-span"><i>y</i></span> is a prime number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i>)</span>.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, each line contains two integers, denoting an edge of the tree. The nodes of the tree are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Output a single integer — the number of triplets that are correct for Furukawa Nagisa's conclusion.</p>





```input1
1 2 1 0
1

```




```input2
3 5 2 1
4 3 1
1 2
2 3

```




```input3
8 13 8 12
0 12 7 4 12 0 8 12
1 8
8 4
4 6
6 2
2 3
8 5
2 7

```




```output1
1

```




```output2
14

```




```output3
341

```


