## Description

<div><p>Duff is one if the heads of Mafia in her country, Andarz Gu. Andarz Gu has <span class="tex-span"><i>n</i></span> cities (numbered from 1 to <span class="tex-span"><i>n</i></span>) connected by <span class="tex-span"><i>m</i></span> bidirectional roads (numbered by <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>).</p><p>Each road has a destructing time, and a color. <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and its color is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and its destructing time is <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Mafia wants to destruct a <span class="tex-font-style-it">matching</span> in Andarz Gu. A <span class="tex-font-style-it">matching</span> is a subset of roads such that no two roads in this subset has common endpoint. They can destruct these roads in parallel, i. e. the total destruction time is a maximum over destruction times of all selected roads.</p><center> <img class="tex-graphics" src="file://j0SLphIH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>They want two conditions to be satisfied:</p><ol> <li> The remaining roads form a <span class="tex-font-style-it">proper coloring</span>. </li><li> Destructing time of this matching is minimized. </li></ol><p>The remaining roads after destructing this matching form a <span class="tex-font-style-it">proper coloring</span> if and only if no two roads of the same color have same endpoint, or, in the other words, edges of each color should form a <span class="tex-font-style-it">matching</span>.</p><p>There is no programmer in Mafia. That's why Duff asked for your help. Please help her and determine which matching to destruct in order to satisfied those conditions (or state that this is not possible).</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5 × 10<sup class="upper-index">4</sup></span> and <span class="tex-span">1 ≤ <i>m</i> ≤ 5 × 10<sup class="upper-index">4</sup></span>), number of cities and number of roads in the country.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the the roads. <span class="tex-span"><i>i</i> - <i>th</i></span> of them contains four integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p></div><div class="output-specification"><p>In the first line of input, print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if satisfying the first condition is possible and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>If it is possible, then you have to print two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> in the second line, the minimum destructing time and the number of roads in the matching (<img align="middle" class="tex-formula" src="file://vJR2HqSE.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>In the third line print <span class="tex-span"><i>k</i></span> distinct integers separated by spaces, indices of the roads in the matching in any order. Roads are numbered starting from one in order of their appearance in the input.</p><p>If there's more than one solution, print any of them.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5 × 10<sup class="upper-index">4</sup></span> and <span class="tex-span">1 ≤ <i>m</i> ≤ 5 × 10<sup class="upper-index">4</sup></span>), number of cities and number of roads in the country.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the the roads. <span class="tex-span"><i>i</i> - <i>th</i></span> of them contains four integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p>

## Output

<p>In the first line of input, print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if satisfying the first condition is possible and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p><p>If it is possible, then you have to print two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> in the second line, the minimum destructing time and the number of roads in the matching (<img align="middle" class="tex-formula" src="file://vJR2HqSE.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>In the third line print <span class="tex-span"><i>k</i></span> distinct integers separated by spaces, indices of the roads in the matching in any order. Roads are numbered starting from one in order of their appearance in the input.</p><p>If there's more than one solution, print any of them.</p>





```input1
5 7
2 1 3 7
3 1 1 6
5 4 1 8
4 5 1 1
3 2 2 3
4 5 2 5
2 3 2 4

```




```input2
3 5
3 2 1 3
1 3 1 1
3 2 1 4
1 3 2 2
1 3 2 10

```




```output1
Yes
3 2
4 5

```




```output2
No

```



## Note

<p>Graph of Andarz Gu in the first sample case is as follows:</p><center> <img class="tex-graphics" src="file://pWBqJ57F.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A solution would be to destruct the roads with crosses.</p><p>Graph of Andarz Gu in the second sample case is as follows:</p><center> <img class="tex-graphics" src="file://HRst41Ej.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
