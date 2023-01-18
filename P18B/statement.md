## Description

<div><p>In one one-dimensional world there are <span class="tex-span"><i>n</i></span> platforms. Platform with index <span class="tex-span"><i>k</i></span> (platforms are numbered from 1) is a segment with coordinates <span class="tex-span">[(<i>k</i> - 1)<i>m</i>, (<i>k</i> - 1)<i>m</i> + <i>l</i>]</span>, and <span class="tex-span"><i>l</i> &lt; <i>m</i></span>. Grasshopper Bob starts to jump along the platforms from point <span class="tex-span">0</span>, with each jump he moves exactly <span class="tex-span"><i>d</i></span> units right. Find out the coordinate of the point, where Bob will fall down. The grasshopper falls down, if he finds himself not on the platform, but if he finds himself on the edge of the platform, he doesn't fall down.</p></div><div class="input-specification"><p>The first input line contains 4 integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i>, <i>m</i>, <i>l</i> ≤ 10<sup class="upper-index">6</sup>, <i>l</i> &lt; <i>m</i></span>) — respectively: amount of platforms, length of the grasshopper Bob's jump, and numbers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>l</i></span> needed to find coordinates of the <span class="tex-span"><i>k</i></span>-th platform: <span class="tex-span">[(<i>k</i> - 1)<i>m</i>, (<i>k</i> - 1)<i>m</i> + <i>l</i>]</span>.</p></div><div class="output-specification"><p>Output the coordinates of the point, where the grosshopper will fall down. Don't forget that if Bob finds himself on the platform edge, he doesn't fall down.</p></div>

## Input

<p>The first input line contains 4 integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i>, <i>m</i>, <i>l</i> ≤ 10<sup class="upper-index">6</sup>, <i>l</i> &lt; <i>m</i></span>) — respectively: amount of platforms, length of the grasshopper Bob's jump, and numbers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>l</i></span> needed to find coordinates of the <span class="tex-span"><i>k</i></span>-th platform: <span class="tex-span">[(<i>k</i> - 1)<i>m</i>, (<i>k</i> - 1)<i>m</i> + <i>l</i>]</span>.</p>

## Output

<p>Output the coordinates of the point, where the grosshopper will fall down. Don't forget that if Bob finds himself on the platform edge, he doesn't fall down.</p>





```input1
2 2 5 3

```




```input2
5 4 11 8

```




```output1
4

```




```output2
20

```


