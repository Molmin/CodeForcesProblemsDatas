## Description

<div><p>One Khanate had a lot of roads and very little wood. Riding along the roads was inconvenient, because the roads did not have road signs indicating the direction to important cities.</p><p>The Han decided that it's time to fix the issue, and ordered to put signs on every road. The Minister of Transport has to do that, but he has only <span class="tex-span"><i>k</i></span> signs. Help the minister to solve his problem, otherwise the poor guy can lose not only his position, but also his head.</p><p>More formally, every road in the Khanate is a line on the <span class="tex-span"><i>Oxy</i></span> plane, given by an equation of the form <span class="tex-span"><i>Ax</i> + <i>By</i> + <i>C</i> = 0</span> (<span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are not equal to 0 at the same time). You are required to determine whether you can put signs in at most <span class="tex-span"><i>k</i></span> points so that each road had at least one sign installed.</p></div><div class="input-specification"><p>The input starts with two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 5</span>)</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integers each, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>, <i>B</i><sub class="lower-index"><i>i</i></sub>, <i>C</i><sub class="lower-index"><i>i</i></sub></span>, the coefficients of the equation that determines the road (<span class="tex-span">|<i>A</i><sub class="lower-index"><i>i</i></sub>|, |<i>B</i><sub class="lower-index"><i>i</i></sub>|, |<i>C</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>B</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> ≠ 0</span>).</p><p>It is guaranteed that no two roads coincide.</p></div><div class="output-specification"><p>If there is no solution, print <span class="tex-font-style-tt">"NO"</span> in the single line (without the quotes).</p><p>Otherwise, print in the first line <span class="tex-font-style-tt">"YES"</span> (without the quotes).</p><p>In the second line print a single number <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ <i>k</i></span>) — the number of used signs. In the next <span class="tex-span"><i>m</i></span> lines print the descriptions of their locations.</p><p>Description of a location of one sign is two integers <span class="tex-span"><i>v</i>, <i>u</i></span>. If <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are two distinct integers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, we assume that sign is at the point of intersection of roads number <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>. If <span class="tex-span"><i>u</i> =  - 1</span>, and <span class="tex-span"><i>v</i></span> is an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, then the sign is on the road number <span class="tex-span"><i>v</i></span> in the point not lying on any other road. In any other case the description of a sign will be assumed invalid and your answer will be considered incorrect. In case if <span class="tex-span"><i>v</i> = <i>u</i></span>, or if <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> are the numbers of two non-intersecting roads, your answer will also be considered incorrect.</p><p>The roads are numbered starting from <span class="tex-span">1</span> in the order in which they follow in the input.</p></div>

## Input

<p>The input starts with two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 5</span>)</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integers each, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub>, <i>B</i><sub class="lower-index"><i>i</i></sub>, <i>C</i><sub class="lower-index"><i>i</i></sub></span>, the coefficients of the equation that determines the road (<span class="tex-span">|<i>A</i><sub class="lower-index"><i>i</i></sub>|, |<i>B</i><sub class="lower-index"><i>i</i></sub>|, |<i>C</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>B</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> ≠ 0</span>).</p><p>It is guaranteed that no two roads coincide.</p>

## Output

<p>If there is no solution, print <span class="tex-font-style-tt">"NO"</span> in the single line (without the quotes).</p><p>Otherwise, print in the first line <span class="tex-font-style-tt">"YES"</span> (without the quotes).</p><p>In the second line print a single number <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ <i>k</i></span>) — the number of used signs. In the next <span class="tex-span"><i>m</i></span> lines print the descriptions of their locations.</p><p>Description of a location of one sign is two integers <span class="tex-span"><i>v</i>, <i>u</i></span>. If <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are two distinct integers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, we assume that sign is at the point of intersection of roads number <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>. If <span class="tex-span"><i>u</i> =  - 1</span>, and <span class="tex-span"><i>v</i></span> is an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, then the sign is on the road number <span class="tex-span"><i>v</i></span> in the point not lying on any other road. In any other case the description of a sign will be assumed invalid and your answer will be considered incorrect. In case if <span class="tex-span"><i>v</i> = <i>u</i></span>, or if <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> are the numbers of two non-intersecting roads, your answer will also be considered incorrect.</p><p>The roads are numbered starting from <span class="tex-span">1</span> in the order in which they follow in the input.</p>





```input1
3 1
1 0 0
0 -1 0
7 -93 0

```




```input2
3 1
1 0 0
0 1 0
1 1 3

```




```input3
2 3
3 4 5
5 6 7

```




```output1
YES
1
1 2

```




```output2
NO

```




```output3
YES
2
1 -1
2 -1

```



## Note

<p>Note that you do not have to minimize <span class="tex-span"><i>m</i></span>, but it shouldn't be more than <span class="tex-span"><i>k</i></span>.</p><p>In the first test all three roads intersect at point (0,0).</p><p>In the second test all three roads form a triangle and there is no way to place one sign so that it would stand on all three roads at once.</p>
