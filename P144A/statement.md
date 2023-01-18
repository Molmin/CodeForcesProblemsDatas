## Description

<div><p>A Ministry for Defense sent a general to inspect the Super Secret Military Squad under the command of the Colonel SuperDuper. Having learned the news, the colonel ordered to all <span class="tex-span"><i>n</i></span> squad soldiers to line up on the parade ground.</p><p>By the military charter the soldiers should stand in the order of non-increasing of their height. But as there's virtually no time to do that, the soldiers lined up in the arbitrary order. However, the general is rather short-sighted and he thinks that the soldiers lined up correctly if the first soldier in the line has the maximum height and the last soldier has the minimum height. Please note that the way other solders are positioned does not matter, including the case when there are several soldiers whose height is maximum or minimum. Only the heights of the <span class="tex-font-style-bf">first</span> and the <span class="tex-font-style-bf">last</span> soldier are important.</p><p>For example, the general considers the sequence of heights <span class="tex-font-style-tt">(4, 3, 4, 2, 1, 1)</span> correct and the sequence <span class="tex-font-style-tt">(4, 3, 1, 2, 2)</span> wrong.</p><p>Within one second the colonel can swap any two neighboring soldiers. Help him count the minimum time needed to form a line-up which the general will consider correct.</p></div><div class="input-specification"><p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) which represents the number of soldiers in the line. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the values of the soldiers' heights in the order of soldiers' heights' increasing in the order from the beginning of the line to its end. The numbers are space-separated. Numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are not necessarily different.</p></div><div class="output-specification"><p>Print the only integer — the minimum number of seconds the colonel will need to form a line-up the general will like.</p></div>

## Input

<p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) which represents the number of soldiers in the line. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the values of the soldiers' heights in the order of soldiers' heights' increasing in the order from the beginning of the line to its end. The numbers are space-separated. Numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are not necessarily different.</p>

## Output

<p>Print the only integer — the minimum number of seconds the colonel will need to form a line-up the general will like.</p>





```input1
4
33 44 11 22

```




```input2
7
10 10 58 31 63 40 76

```




```output1
2

```




```output2
10

```



## Note

<p>In the first sample the colonel will need to swap the first and second soldier and then the third and fourth soldier. That will take 2 seconds. The resulting position of the soldiers is <span class="tex-font-style-tt">(44, 33, 22, 11)</span>.</p><p>In the second sample the colonel may swap the soldiers in the following sequence:</p><ol> <li> <span class="tex-font-style-tt">(10, 10, 58, 31, 63, 40, 76)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 10, 31, 63, 40, 76)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 10, 31, 63, 76, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 10, 31, 76, 63, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 31, 10, 76, 63, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 31, 76, 10, 63, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 31, 76, 63, 10, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 58, 76, 31, 63, 10, 40)</span> </li><li> <span class="tex-font-style-tt">(10, 76, 58, 31, 63, 10, 40)</span> </li><li> <span class="tex-font-style-tt">(76, 10, 58, 31, 63, 10, 40)</span> </li><li> <span class="tex-font-style-tt">(76, 10, 58, 31, 63, 40, 10)</span> </li></ol>
