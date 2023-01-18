## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in Berland. Each city has its index — an integer number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The capital has index <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>. All the roads in Berland are two-way. The road system is such that there is exactly one path from the capital to each city, i.e. the road map looks like a tree. In Berland's chronicles the road map is kept in the following way: for each city <span class="tex-span"><i>i</i></span>, different from the capital, there is kept number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — index of the last city on the way from the capital to <span class="tex-span"><i>i</i></span>.</p><p>Once the king of Berland Berl XXXIV decided to move the capital from city <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> to city <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>. Naturally, after this the old representation of the road map in Berland's chronicles became incorrect. Please, help the king find out a new representation of the road map in the way described above.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup>, 1 ≤ <i>r</i><sub class="lower-index">1</sub> ≠ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>) — amount of cities in Berland, index of the old capital and index of the new one, correspondingly.</p><p>The following line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers — the old representation of the road map. For each city, apart from <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, there is given integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — index of the last city on the way from the capital to city <span class="tex-span"><i>i</i></span>. All the cities are described in order of increasing indexes.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> - 1</span> numbers — new representation of the road map in the same format.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup>, 1 ≤ <i>r</i><sub class="lower-index">1</sub> ≠ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>) — amount of cities in Berland, index of the old capital and index of the new one, correspondingly.</p><p>The following line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers — the old representation of the road map. For each city, apart from <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, there is given integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — index of the last city on the way from the capital to city <span class="tex-span"><i>i</i></span>. All the cities are described in order of increasing indexes.</p>

## Output

<p>Output <span class="tex-span"><i>n</i> - 1</span> numbers — new representation of the road map in the same format.</p>





```input1
3 2 3
2 2

```




```input2
6 2 4
6 1 2 4 2

```




```output1
2 3
```




```output2
6 4 1 4 2
```


