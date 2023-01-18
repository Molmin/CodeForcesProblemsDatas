## Description

<div><p>The Fat Rat and his friend Сerealguy have had a bet whether at least a few oats are going to descend to them by some clever construction. The figure below shows the clever construction.</p><center> <img class="tex-graphics" src="file://foEYF8eG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A more formal description of the clever construction is as follows. The clever construction consists of <span class="tex-span"><i>n</i></span> rows with scales. The first row has <span class="tex-span"><i>n</i></span> scales, the second row has <span class="tex-span">(<i>n</i> - 1)</span> scales, the <span class="tex-span"><i>i</i></span>-th row has <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span> scales, the last row has exactly one scale. Let's number the scales in each row from the left to the right, starting from <span class="tex-span">1</span>. Then the value of <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> in kilograms <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>k</i> ≤ <i>n</i> - <i>i</i> + 1)</span> is the weight capacity parameter of the <span class="tex-span"><i>k</i></span>-th scale in the <span class="tex-span"><i>i</i></span>-th row. </p><p>If a body whose mass is not less than <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> falls on the scale with weight capacity <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>, then the scale breaks. At that anything that the scale has on it, either falls one level down to the left (if possible) or one level down to the right (if possible). In other words, if the scale <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> <span class="tex-span">(<i>i</i> &lt; <i>n</i>)</span> breaks, then there are at most two possible variants in which the contents of the scale's pan can fall out: <span class="tex-font-style-bf">all contents</span> of scale <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> falls either on scale <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i> + 1, <i>k</i> - 1</sub></span> (if it exists), or on scale <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i> + 1, <i>k</i></sub></span> (if it exists). If scale <span class="tex-span"><i>w</i><sub class="lower-index"><i>n</i>, 1</sub></span> breaks, then all its contents falls right in the Fat Rat's claws. Please note that the scales that are the first and the last in a row, have only one variant of dropping the contents.</p><p>Initially, oats are simultaneously put on all scales of the first level. The <span class="tex-span"><i>i</i></span>-th scale has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of oats put on it. After that the scales start breaking and the oats start falling down in some way. You can consider everything to happen instantly. That is, the scale breaks instantly and the oats also fall instantly.</p><p>The Fat Rat is sure that whatever happens, he will not get the oats from the first level. Cerealguy is sure that there is such a scenario, when the rat gets at least some number of the oats. Help the Fat Rat and the Cerealguy. Determine, which one is right.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of rows with scales.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the masses of the oats in kilograms.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain descriptions of the scales: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span> space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the weight capacity parameters for the scales that stand on the <span class="tex-span"><i>i</i></span>-th row, in kilograms.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Fat Rat</span>" if the Fat Rat is right, otherwise print "<span class="tex-font-style-tt">Cerealguy</span>".</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of rows with scales.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the masses of the oats in kilograms.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain descriptions of the scales: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span> space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the weight capacity parameters for the scales that stand on the <span class="tex-span"><i>i</i></span>-th row, in kilograms.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Fat Rat</span>" if the Fat Rat is right, otherwise print "<span class="tex-font-style-tt">Cerealguy</span>".</p>





```input1
1
1
2

```




```input2
2
2 2
1 2
4

```




```input3
2
2 2
1 2
5

```




```output1
Fat Rat

```




```output2
Cerealguy

```




```output3
Fat Rat

```



## Note

<p>Notes to the examples: </p><ul> <li> The first example: the scale with weight capacity 2 gets 1. That means that the lower scale don't break. </li><li> The second sample: all scales in the top row obviously break. Then the oats fall on the lower row. Their total mass is 4,and that's exactly the weight that the lower scale can "nearly endure". So, as 4 <span class="tex-span"> ≥ </span> 4, the scale breaks.</li></ul>
