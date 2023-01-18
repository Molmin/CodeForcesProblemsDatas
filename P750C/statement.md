## Description

<div><p>Every Codeforces user has rating, described with one integer, possibly negative or zero. Users are divided into two divisions. The first division is for users with rating <span class="tex-span">1900</span> or higher. Those with rating <span class="tex-span">1899</span> or lower belong to the second division. In every contest, according to one's performance, his or her rating changes by some value, possibly negative or zero.</p><p>Limak competed in <span class="tex-span"><i>n</i></span> contests in the year 2016. He remembers that in the <span class="tex-span"><i>i</i></span>-th contest he competed in the division <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (i.e. he belonged to this division <span class="tex-font-style-bf">just before</span> the start of this contest) and his rating changed by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-bf">just after the contest</span>. Note that negative <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> denotes the loss of rating.</p><p>What is the maximum possible rating Limak can have right now, after all <span class="tex-span"><i>n</i></span> contests? If his rating may be arbitrarily big, print "<span class="tex-font-style-tt">Infinity</span>". If there is no scenario matching the given information, print "<span class="tex-font-style-tt">Impossible</span>".</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), describing Limak's rating change after the <span class="tex-span"><i>i</i></span>-th contest and his division during the <span class="tex-span"><i>i</i></span>-th contest contest.</p></div><div class="output-specification"><p>If Limak's current rating can be arbitrarily big, print "<span class="tex-font-style-tt">Infinity</span>" (without quotes). If the situation is impossible, print "<span class="tex-font-style-tt">Impossible</span>" (without quotes). Otherwise print one integer, denoting the maximum possible value of Limak's current rating, i.e. rating after the <span class="tex-span"><i>n</i></span> contests.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), describing Limak's rating change after the <span class="tex-span"><i>i</i></span>-th contest and his division during the <span class="tex-span"><i>i</i></span>-th contest contest.</p>

## Output

<p>If Limak's current rating can be arbitrarily big, print "<span class="tex-font-style-tt">Infinity</span>" (without quotes). If the situation is impossible, print "<span class="tex-font-style-tt">Impossible</span>" (without quotes). Otherwise print one integer, denoting the maximum possible value of Limak's current rating, i.e. rating after the <span class="tex-span"><i>n</i></span> contests.</p>





```input1
3
-7 1
5 2
8 2

```




```input2
2
57 1
22 2

```




```input3
1
-5 1

```




```input4
4
27 2
13 1
-50 1
8 2

```




```output1
1907

```




```output2
Impossible

```




```output3
Infinity

```




```output4
1897

```



## Note

<p>In the first sample, the following scenario matches all information Limak remembers and has maximum possible final rating:</p><ul> <li> Limak has rating <span class="tex-span">1901</span> and belongs to the division <span class="tex-span">1</span> in the first contest. His rating decreases by <span class="tex-span">7</span>. </li><li> With rating <span class="tex-span">1894</span> Limak is in the division <span class="tex-span">2</span>. His rating increases by <span class="tex-span">5</span>. </li><li> Limak has rating <span class="tex-span">1899</span> and is still in the division <span class="tex-span">2</span>. In the last contest of the year he gets <span class="tex-span"> + 8</span> and ends the year with rating <span class="tex-span">1907</span>. </li></ul><p>In the second sample, it's impossible that Limak is in the division <span class="tex-span">1</span>, his rating increases by <span class="tex-span">57</span> and after that Limak is in the division <span class="tex-span">2</span> in the second contest.</p>
