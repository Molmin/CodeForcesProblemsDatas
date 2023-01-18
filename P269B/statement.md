## Description

<div><p>Emuskald is an avid horticulturist and owns the world's longest greenhouse — it is effectively infinite in length.</p><p>Over the years Emuskald has cultivated <span class="tex-span"><i>n</i></span> plants in his greenhouse, of <span class="tex-span"><i>m</i></span> different plant species numbered from 1 to <span class="tex-span"><i>m</i></span>. His greenhouse is very narrow and can be viewed as an infinite line, with each plant occupying a single point on that line.</p><p>Emuskald has discovered that each species thrives at a different temperature, so he wants to arrange <span class="tex-span"><i>m</i> - 1</span> borders that would divide the greenhouse into <span class="tex-span"><i>m</i></span> sections numbered from 1 to <span class="tex-span"><i>m</i></span> from left to right with each section housing a single species. He is free to place the borders, but in the end all of the <span class="tex-span"><i>i</i></span>-th species plants must reside in <span class="tex-span"><i>i</i></span>-th section from the left.</p><p>Of course, it is not always possible to place the borders in such way, so Emuskald needs to replant some of his plants. He can remove each plant from its position and place it anywhere in the greenhouse (at <span class="tex-font-style-bf">any</span> real coordinate) with no plant already in it. Since replanting is a lot of stress for the plants, help Emuskald find the minimum number of plants he has to replant to be able to place the borders.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>, <span class="tex-span"><i>n</i> ≥ <i>m</i></span>), the number of plants and the number of different species. Each of the following <span class="tex-span"><i>n</i></span> lines contain two space-separated numbers: one integer number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), and one real number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the species and position of the <span class="tex-span"><i>i</i></span>-th plant. Each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will contain no more than 6 digits after the decimal point.</p><p>It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different; there is at least one plant of each species; the plants are given in order "from left to the right", that is in the ascending order of their <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>, 1 ≤ <i>i</i> &lt; <i>n</i>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the minimum number of plants to be replanted.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>, <span class="tex-span"><i>n</i> ≥ <i>m</i></span>), the number of plants and the number of different species. Each of the following <span class="tex-span"><i>n</i></span> lines contain two space-separated numbers: one integer number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), and one real number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the species and position of the <span class="tex-span"><i>i</i></span>-th plant. Each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will contain no more than 6 digits after the decimal point.</p><p>It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different; there is at least one plant of each species; the plants are given in order "from left to the right", that is in the ascending order of their <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>, 1 ≤ <i>i</i> &lt; <i>n</i>)</span>.</p>

## Output

<p>Output a single integer — the minimum number of plants to be replanted.</p>





```input1
3 2
2 1
1 2.0
1 3.100

```




```input2
3 3
1 5.0
2 5.5
3 6.0

```




```input3
6 3
1 14.284235
2 17.921382
1 20.328172
3 20.842331
1 25.790145
1 27.204125

```




```output1
1

```




```output2
0

```




```output3
2

```



## Note

<p>In the first test case, Emuskald can replant the first plant to the right of the last plant, so the answer is 1.</p><p>In the second test case, the species are already in the correct order, so no replanting is needed.</p>
