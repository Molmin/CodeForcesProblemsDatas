## Description

<div><p>John Doe has a crooked fence, consisting of <span class="tex-span"><i>n</i></span> rectangular planks, lined up from the left to the right: the plank that goes <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> (from left to right) has width 1 and height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. We will assume that the plank that goes <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> (from left to right) has index <span class="tex-span"><i>i</i></span>.</p><p>A <span class="tex-font-style-it">piece of the fence</span> from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> is a sequence of planks of wood with indices from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive, that is, planks with indices <span class="tex-span"><i>l</i>, <i>l</i> + 1, ..., <i>r</i></span>. The width of the piece of the fence from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> is value <span class="tex-span"><i>r</i> - <i>l</i> + 1</span>.</p><p>Two pieces of the fence from <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and from <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> are called matching, if the following conditions hold:</p><ul> <li> the pieces do not intersect, that is, there isn't a single plank, such that it occurs in both pieces of the fence; </li><li> the pieces are of the same width; </li><li> for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(0 ≤ <i>i</i> ≤ <i>r</i><sub class="lower-index">1</sub> - <i>l</i><sub class="lower-index">1</sub>)</span> the following condition holds: <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i><sub class="lower-index">1</sub> + <i>i</i></sub> + <i>h</i><sub class="lower-index"><i>l</i><sub class="lower-index">2</sub> + <i>i</i></sub> = <i>h</i><sub class="lower-index"><i>l</i><sub class="lower-index">1</sub></sub> + <i>h</i><sub class="lower-index"><i>l</i><sub class="lower-index">2</sub></sub></span>. </li></ul><p>John chose a few pieces of the fence and now wants to know how many distinct matching pieces are for each of them. Two pieces of the fence are distinct if there is a plank, which belongs to one of them and does not belong to the other one.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of wood planks in the fence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of fence planks.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the boundaries of the <span class="tex-span"><i>i</i></span>-th piece of the fence.</p></div><div class="output-specification"><p>For each query on a single line print a single integer — the number of pieces of the fence that match the given one. Print the answers to the queries in the order, in which the queries are given in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of wood planks in the fence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of fence planks.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the boundaries of the <span class="tex-span"><i>i</i></span>-th piece of the fence.</p>

## Output

<p>For each query on a single line print a single integer — the number of pieces of the fence that match the given one. Print the answers to the queries in the order, in which the queries are given in the input.</p>





```input1
10
1 2 2 1 100 99 99 100 100 100
6
1 4
1 2
3 4
1 5
9 10
10 10

```




```output1
1
2
2
0
2
9

```


