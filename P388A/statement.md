## Description

<div><p>Fox Ciel has <span class="tex-span"><i>n</i></span> boxes in her room. They have the same size and weight, but they might have different strength. The <span class="tex-span"><i>i</i></span>-th box can hold at most <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> boxes on its top (we'll call <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> the strength of the box). </p><p>Since all the boxes have the same size, Ciel cannot put more than one box directly on the top of some box. For example, imagine Ciel has three boxes: the first has strength 2, the second has strength 1 and the third has strength 1. She cannot put the second and the third box simultaneously directly on the top of the first one. But she can put the second box directly on the top of the first one, and then the third box directly on the top of the second one. We will call such a construction of boxes a <span class="tex-font-style-it">pile</span>.</p><center><img class="tex-graphics" src="file://OQ3qlZYk.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Fox Ciel wants to construct piles from all the boxes. Each pile will contain some boxes from top to bottom, and there cannot be more than <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> boxes on the top of <span class="tex-span"><i>i</i></span>-th box. What is the minimal number of piles she needs to construct?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Output a single integer — the minimal possible number of piles.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Output a single integer — the minimal possible number of piles.</p>





```input1
3
0 0 10

```




```input2
5
0 1 2 3 4

```




```input3
4
0 0 0 0

```




```input4
9
0 1 0 2 0 1 1 2 10

```




```output1
2

```




```output2
1

```




```output3
4

```




```output4
3

```



## Note

<p>In example 1, one optimal way is to build 2 piles: the first pile contains boxes 1 and 3 (from top to bottom), the second pile contains only box 2.</p><center><img class="tex-graphics" src="file://f9uFh208.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In example 2, we can build only 1 pile that contains boxes 1, 2, 3, 4, 5 (from top to bottom).</p><center><img class="tex-graphics" src="file://aBmDi6kj.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
