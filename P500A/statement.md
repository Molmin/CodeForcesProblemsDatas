## Description

<div><p>New Year is coming in Line World! In this world, there are <span class="tex-span"><i>n</i></span> cells numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, as a <span class="tex-span">1 × <i>n</i></span> board. People live in cells. However, it was hard to move between distinct cells, because of the difficulty of escaping the cell. People wanted to meet people who live in other cells.</p><p>So, user tncks0121 has made a transportation system to move between these cells, to celebrate the New Year. First, he thought of <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. For every integer <span class="tex-span"><i>i</i></span> where <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span> the condition <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>i</i></span> holds. Next, he made <span class="tex-span"><i>n</i> - 1</span> portals, numbered by integers from 1 to <span class="tex-span"><i>n</i> - 1</span>. The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) portal connects cell <span class="tex-span"><i>i</i></span> and cell <span class="tex-span">(<i>i</i> + <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>, and one can travel from cell <span class="tex-span"><i>i</i></span> to cell <span class="tex-span">(<i>i</i> + <i>a</i><sub class="lower-index"><i>i</i></sub>)</span> using the <span class="tex-span"><i>i</i></span>-th portal. Unfortunately, one cannot use the portal backwards, which means one cannot move from cell <span class="tex-span">(<i>i</i> + <i>a</i><sub class="lower-index"><i>i</i></sub>)</span> to cell <span class="tex-span"><i>i</i></span> using the <span class="tex-span"><i>i</i></span>-th portal. It is easy to see that because of condition <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>i</i></span> one can't leave the Line World using portals.</p><p>Currently, I am standing at cell <span class="tex-span">1</span>, and I want to go to cell <span class="tex-span"><i>t</i></span>. However, I don't know whether it is possible to go there. Please determine whether I can go to cell <span class="tex-span"><i>t</i></span> by only using the construted transportation system.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3 × 10<sup class="upper-index">4</sup></span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>t</i> ≤ <i>n</i></span>) — the number of cells, and the index of the cell which I want to go to.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>i</i></span>). It is guaranteed, that using the given transportation system, one cannot leave the Line World.</p></div><div class="output-specification"><p>If I can go to cell <span class="tex-span"><i>t</i></span> using the transportation system, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3 × 10<sup class="upper-index">4</sup></span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>t</i> ≤ <i>n</i></span>) — the number of cells, and the index of the cell which I want to go to.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>i</i></span>). It is guaranteed, that using the given transportation system, one cannot leave the Line World.</p>

## Output

<p>If I can go to cell <span class="tex-span"><i>t</i></span> using the transportation system, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
8 4
1 2 1 2 1 2 1

```




```input2
8 5
1 2 1 2 1 1 1

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, the visited cells are: <span class="tex-span">1, 2, 4</span>; so we can successfully visit the cell <span class="tex-span">4</span>.</p><p>In the second sample, the possible cells to visit are: <span class="tex-span">1, 2, 4, 6, 7, 8</span>; so we can't visit the cell <span class="tex-span">5</span>, which we want to visit.</p>
