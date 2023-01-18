## Description

<div><p>Andrewid the Android is a galaxy-famous detective. He is now chasing a criminal hiding on the planet Oxa-5, the planet almost fully covered with water.</p><p>The only dry land there is an archipelago of <span class="tex-span"><i>n</i></span> narrow islands located in a row. For more comfort let's represent them as non-intersecting segments on a straight line: island <span class="tex-span"><i>i</i></span> has coordinates <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>, besides, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &lt; <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>.</p><p>To reach the goal, Andrewid needs to place a bridge between each pair of <span class="tex-font-style-bf">adjacent</span> islands. A bridge of length <span class="tex-span"><i>a</i></span> can be placed between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span">(<i>i</i> + 1)</span>-th islads, if there are such coordinates of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, that <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>i</i> + 1</sub></span> and <span class="tex-span"><i>y</i> - <i>x</i> = <i>a</i></span>. </p><p>The detective was supplied with <span class="tex-span"><i>m</i></span> bridges, each bridge can be used at most once. Help him determine whether the bridges he got are enough to connect each pair of adjacent islands.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of islands and bridges.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — the coordinates of the island endpoints.</p><p>The last line contains <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">integer</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — the lengths of the bridges that Andrewid got.</p></div><div class="output-specification"><p>If it is impossible to place a bridge between each pair of adjacent islands in the required manner, print on a single line <span class="tex-font-style-tt">"No"</span> (without the quotes), otherwise print in the first line <span class="tex-font-style-tt">"Yes"</span> (without the quotes), and in the second line print <span class="tex-span"><i>n</i> - 1</span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span>, which mean that between islands <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> there must be used a bridge number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>If there are multiple correct answers, print any of them. Note that in this problem it is necessary to print <span class="tex-font-style-tt">"Yes"</span> and <span class="tex-font-style-tt">"No"</span> in correct case.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of islands and bridges.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — the coordinates of the island endpoints.</p><p>The last line contains <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">integer</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — the lengths of the bridges that Andrewid got.</p>

## Output

<p>If it is impossible to place a bridge between each pair of adjacent islands in the required manner, print on a single line <span class="tex-font-style-tt">"No"</span> (without the quotes), otherwise print in the first line <span class="tex-font-style-tt">"Yes"</span> (without the quotes), and in the second line print <span class="tex-span"><i>n</i> - 1</span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span>, which mean that between islands <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> there must be used a bridge number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>If there are multiple correct answers, print any of them. Note that in this problem it is necessary to print <span class="tex-font-style-tt">"Yes"</span> and <span class="tex-font-style-tt">"No"</span> in correct case.</p>





```input1
4 4
1 4
7 8
9 10
12 14
4 5 3 8

```




```input2
2 2
11 14
17 18
2 9

```




```input3
2 1
1 1
1000000000000000000 1000000000000000000
999999999999999999

```




```output1
Yes
2 3 1 

```




```output2
No

```




```output3
Yes
1 

```



## Note

<p>In the first sample test you can, for example, place the second bridge between points 3 and 8, place the third bridge between points 7 and 10 and place the first bridge between points 10 and 14.</p><p>In the second sample test the first bridge is too short and the second bridge is too long, so the solution doesn't exist.</p>
