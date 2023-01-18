## Description

<div><p>Petya has equal wooden bars of length <span class="tex-span"><i>n</i></span>. He wants to make a frame for <span class="tex-font-style-it">two</span> equal doors. Each frame has two vertical (left and right) sides of length <span class="tex-span"><i>a</i></span> and one top side of length <span class="tex-span"><i>b</i></span>. A solid (i.e. continuous without breaks) piece of bar is needed for each side.</p><p>Determine a minimal number of wooden bars which are needed to make the frames for two doors. Petya can cut the wooden bars into any parts, but each side of each door should be a solid piece of a wooden bar (or a whole wooden bar).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the length of each wooden bar.</p><p>The second line contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>) — the length of the vertical (left and right) sides of a door frame.</p><p>The third line contains a single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i></span>) — the length of the upper side of a door frame.</p></div><div class="output-specification"><p>Print the minimal number of wooden bars with length <span class="tex-span"><i>n</i></span> which are needed to make the frames for two doors.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the length of each wooden bar.</p><p>The second line contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>) — the length of the vertical (left and right) sides of a door frame.</p><p>The third line contains a single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i></span>) — the length of the upper side of a door frame.</p>

## Output

<p>Print the minimal number of wooden bars with length <span class="tex-span"><i>n</i></span> which are needed to make the frames for two doors.</p>





```input1
8
1
2

```




```input2
5
3
4

```




```input3
6
4
2

```




```input4
20
5
6

```




```output1
1

```




```output2
6

```




```output3
4

```




```output4
2

```



## Note

<p>In the first example one wooden bar is enough, since the total length of all six sides of the frames for two doors is <span class="tex-span">8</span>.</p><p>In the second example <span class="tex-span">6</span> wooden bars is enough, because for each side of the frames the new wooden bar is needed.</p>
