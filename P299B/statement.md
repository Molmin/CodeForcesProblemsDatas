## Description

<div><p>Ksusha the Squirrel is standing at the beginning of a straight road, divided into <span class="tex-span"><i>n</i></span> sectors. The sectors are numbered 1 to <span class="tex-span"><i>n</i></span>, from left to right. Initially, Ksusha stands in sector 1. </p><p>Ksusha wants to walk to the end of the road, that is, get to sector <span class="tex-span"><i>n</i></span>. Unfortunately, there are some rocks on the road. We know that Ksusha hates rocks, so she doesn't want to stand in sectors that have rocks.</p><p>Ksusha the squirrel keeps fit. She can jump from sector <span class="tex-span"><i>i</i></span> to any of the sectors <span class="tex-span"><i>i</i> + 1, <i>i</i> + 2, ..., <i>i</i> + <i>k</i></span>. </p><p>Help Ksusha! Given the road description, say if she can reach the end of the road (note, she cannot stand on a rock)?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> characters — the description of the road: the <span class="tex-span"><i>i</i></span>-th character equals "<span class="tex-font-style-tt">.</span>", if the <span class="tex-span"><i>i</i></span>-th sector contains no rocks. Otherwise, it equals "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the first and the last characters equal "<span class="tex-font-style-tt">.</span>".</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if Ksusha can reach the end of the road, otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> characters — the description of the road: the <span class="tex-span"><i>i</i></span>-th character equals "<span class="tex-font-style-tt">.</span>", if the <span class="tex-span"><i>i</i></span>-th sector contains no rocks. Otherwise, it equals "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the first and the last characters equal "<span class="tex-font-style-tt">.</span>".</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if Ksusha can reach the end of the road, otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
2 1
..

```




```input2
5 2
.#.#.

```




```input3
7 3
.#.###.

```




```output1
YES

```




```output2
YES

```




```output3
NO

```


