## Description

<div><p>A new cottage village called «Flatville» is being built in Flatland. By now they have already built in «Flatville» <span class="tex-span"><i>n</i></span> square houses with the centres on the <span class="tex-span"><i>Оx</i></span>-axis. The houses' sides are parallel to the coordinate axes. It's known that no two houses overlap, but they can touch each other.</p><p>The architect bureau, where Peter works, was commissioned to build a new house in «Flatville». The customer wants his future house to be on the <span class="tex-span"><i>Оx</i></span>-axis, to be square in shape, have a side <span class="tex-span"><i>t</i></span>, and touch at least one of the already built houses. For sure, its sides should be parallel to the coordinate axes, its centre should be on the <span class="tex-span"><i>Ox</i></span>-axis and it shouldn't overlap any of the houses in the village.</p><p>Peter was given a list of all the houses in «Flatville». Would you help him find the amount of possible positions of the new house?</p></div><div class="input-specification"><p>The first line of the input data contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 1000</span>). Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains two space-separated integer numbers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — <span class="tex-span"><i>x</i></span>-coordinate of the centre of the <span class="tex-span"><i>i</i></span>-th house, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — length of its side (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output the amount of possible positions of the new house.</p></div>

## Input

<p>The first line of the input data contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 1000</span>). Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains two space-separated integer numbers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — <span class="tex-span"><i>x</i></span>-coordinate of the centre of the <span class="tex-span"><i>i</i></span>-th house, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — length of its side (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>Output the amount of possible positions of the new house.</p>





```input1
2 2
0 4
6 2

```




```input2
2 2
0 4
5 2

```




```input3
2 3
0 4
5 2

```




```output1
4

```




```output2
3

```




```output3
2

```



## Note

<p>It is possible for the <span class="tex-span"><i>x</i></span>-coordinate of the new house to have non-integer value.</p>
