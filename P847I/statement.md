## Description

<div><p>The Berland's capital has the form of a rectangle with sizes <span class="tex-span"><i>n</i> × <i>m</i></span> quarters. All quarters are divided into three types:</p><ul> <li> regular (labeled with the character '<span class="tex-font-style-tt">.</span>') — such quarters do not produce the noise but are not obstacles to the propagation of the noise; </li><li> sources of noise (labeled with an uppercase Latin letter from '<span class="tex-font-style-tt">A</span>' to '<span class="tex-font-style-tt">Z</span>') — such quarters are noise sources and are not obstacles to the propagation of the noise; </li><li> heavily built-up (labeled with the character '<span class="tex-font-style-tt">*</span>') — such quarters are soundproofed, the noise does not penetrate into them and they themselves are obstacles to the propagation of noise. </li></ul><p>A quarter labeled with letter '<span class="tex-font-style-tt">A</span>' produces <span class="tex-span"><i>q</i></span> units of noise. A quarter labeled with letter '<span class="tex-font-style-tt">B</span>' produces <span class="tex-span">2·<i>q</i></span> units of noise. And so on, up to a quarter labeled with letter '<span class="tex-font-style-tt">Z</span>', which produces <span class="tex-span">26·<i>q</i></span> units of noise. There can be any number of quarters labeled with each letter in the city.</p><p>When propagating from the source of the noise, the noise level is halved when moving from one quarter to a quarter that shares a side with it (when an odd number is to be halved, it's rounded down). The noise spreads along the chain. For example, if some quarter is located at a distance <span class="tex-span">2</span> from the noise source, then the value of noise which will reach the quarter is divided by <span class="tex-span">4</span>. So the noise level that comes from the source to the quarter is determined solely by the length of the shortest path between them. Heavily built-up quarters are obstacles, the noise does not penetrate into them.</p><center> <img class="tex-graphics" src="file://1ywseWLm.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The values in the cells of the table on the right show the total noise level in the respective quarters for <span class="tex-span"><i>q</i> = 100</span>, the first term in each sum is the noise from the quarter '<span class="tex-font-style-tt">A</span>', the second — the noise from the quarter '<span class="tex-font-style-tt">B</span>'.</span> </center><p>The noise level in quarter is defined as the sum of the noise from all sources. To assess the quality of life of the population of the capital of Berland, it is required to find the number of quarters whose noise level exceeds the allowed level <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>q</i>, <i>p</i> ≤ 10<sup class="upper-index">6</sup></span>) — the sizes of Berland's capital, the number of noise units that a quarter '<span class="tex-font-style-tt">A</span>' produces, and the allowable noise level.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the capital quarters, in the format that was described in the statement above. It is possible that in the Berland's capital there are no quarters of any type.</p></div><div class="output-specification"><p>Print the number of quarters, in which the noise level exceeds the allowed level <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>q</i>, <i>p</i> ≤ 10<sup class="upper-index">6</sup></span>) — the sizes of Berland's capital, the number of noise units that a quarter '<span class="tex-font-style-tt">A</span>' produces, and the allowable noise level.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the capital quarters, in the format that was described in the statement above. It is possible that in the Berland's capital there are no quarters of any type.</p>

## Output

<p>Print the number of quarters, in which the noise level exceeds the allowed level <span class="tex-span"><i>p</i></span>.</p>





```input1
3 3 100 140
...
A*.
.B.

```




```input2
3 3 2 8
B*.
BB*
BBB

```




```input3
3 4 5 4
..*B
..**
D...

```




```output1
3

```




```output2
4

```




```output3
7

```



## Note

<p>The illustration to the first example is in the main part of the statement.</p>
