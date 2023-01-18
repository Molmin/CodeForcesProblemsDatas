## Description

<div><p>The game of bingo is played on a <span class="tex-span">5 × 5</span> square grid filled with distinct numbers between <span class="tex-span">1</span> and <span class="tex-span">75</span>. In this problem you will consider a generalized version played on an <span class="tex-span"><i>n</i> × <i>n</i></span> grid with distinct numbers between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> ≥ <i>n</i><sup class="upper-index">2</sup>)</span>. </p><p>A player begins by selecting a randomly generated bingo grid (generated uniformly among all available grids). Then <span class="tex-span"><i>k</i></span> distinct numbers between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span> will be called at random (called uniformly among all available sets of <span class="tex-span"><i>k</i></span> numbers). For each called number that appears on the grid, the player marks that cell. The score at the end is 2 raised to the power of (number of completely marked rows plus number of completely marked columns).</p><p>Determine the expected value of the score. The expected score may be very large. If the expected score is larger than <span class="tex-span">10<sup class="upper-index">99</sup></span>, print <span class="tex-span">10<sup class="upper-index">99</sup></span> instead (for example as "<span class="tex-font-style-tt">1e99</span>" without the quotes).</p></div><div class="input-specification"><p>Input will consist of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300;&nbsp;<i>n</i><sup class="upper-index">2</sup> ≤ <i>m</i> ≤ 100000;&nbsp;<i>n</i> ≤ <i>k</i> ≤ <i>m</i>)</span>.</p></div><div class="output-specification"><p>Print the smaller of <span class="tex-span">10<sup class="upper-index">99</sup></span> and the expected score. Your answer must be correct within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>Input will consist of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 300;&nbsp;<i>n</i><sup class="upper-index">2</sup> ≤ <i>m</i> ≤ 100000;&nbsp;<i>n</i> ≤ <i>k</i> ≤ <i>m</i>)</span>.</p>

## Output

<p>Print the smaller of <span class="tex-span">10<sup class="upper-index">99</sup></span> and the expected score. Your answer must be correct within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 2 1

```




```input2
2 4 3

```




```input3
7 59164 40872

```




```output1
2.5

```




```output2
4

```




```output3
3.1415926538

```


