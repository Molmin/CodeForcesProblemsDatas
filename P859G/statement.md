## Description

<div><p><span class="tex-span"><i>n</i></span> evenly spaced points have been marked around the edge of a circle. There is a number written at each point. You choose a positive real number <span class="tex-span"><i>k</i></span>. Then you may repeatedly select a set of <span class="tex-span">2</span> or more points which are evenly spaced, and either increase all numbers at points in the set by <span class="tex-span"><i>k</i></span> or decrease all numbers at points in the set by <span class="tex-span"><i>k</i></span>. You would like to eventually end up with all numbers equal to <span class="tex-span">0</span>. Is it possible?</p><p>A set of <span class="tex-span">2</span> points is considered evenly spaced if they are diametrically opposed, and a set of <span class="tex-span">3</span> or more points is considered evenly spaced if they form a regular polygon.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>), the number of points along the circle.</p><p>The following line contains a string <span class="tex-span"><i>s</i></span> with exactly <span class="tex-span"><i>n</i></span> digits, indicating the numbers initially present at each of the points, in clockwise order.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is some sequence of operations that results in all numbers being <span class="tex-span">0</span>, otherwise "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>), the number of points along the circle.</p><p>The following line contains a string <span class="tex-span"><i>s</i></span> with exactly <span class="tex-span"><i>n</i></span> digits, indicating the numbers initially present at each of the points, in clockwise order.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is some sequence of operations that results in all numbers being <span class="tex-span">0</span>, otherwise "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>





```input1
30
000100000100000110000000001100

```




```input2
6
314159

```




```output1
YES

```




```output2
NO

```



## Note

<p>If we label the points from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, then for the first test case we can set <span class="tex-span"><i>k</i> = 1</span>. Then we increase the numbers at points <span class="tex-span">7</span> and <span class="tex-span">22</span> by <span class="tex-span">1</span>, then decrease the numbers at points <span class="tex-span">7</span>, <span class="tex-span">17</span>, and <span class="tex-span">27</span> by <span class="tex-span">1</span>, then decrease the numbers at points <span class="tex-span">4</span>, <span class="tex-span">10</span>, <span class="tex-span">16</span>, <span class="tex-span">22</span>, and <span class="tex-span">28</span> by <span class="tex-span">1</span>.</p>
