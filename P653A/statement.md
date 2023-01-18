## Description

<div><p>Limak is a little polar bear. He has <span class="tex-span"><i>n</i></span> balls, the <span class="tex-span"><i>i</i></span>-th ball has size <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Limak wants to give one ball to each of his three friends. Giving gifts isn't easy&nbsp;— there are two rules Limak must obey to make friends happy:</p><ul> <li> No two friends can get balls of the same size. </li><li> No two friends can get balls of sizes that differ by more than <span class="tex-span">2</span>. </li></ul><p>For example, Limak can choose balls with sizes <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">3</span>, or balls with sizes <span class="tex-span">90</span>, <span class="tex-span">91</span> and <span class="tex-span">92</span>. But he can't choose balls with sizes <span class="tex-span">5</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span> (two friends would get balls of the same size), and he can't choose balls with sizes <span class="tex-span">30</span>, <span class="tex-span">31</span> and <span class="tex-span">33</span> (because sizes <span class="tex-span">30</span> and <span class="tex-span">33</span> differ by more than <span class="tex-span">2</span>).</p><p>Your task is to check whether Limak can choose three balls that satisfy conditions above.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of balls Limak has.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the size of the <span class="tex-span"><i>i</i></span>-th ball.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Limak can choose three balls of distinct sizes, such that any two of them differ by no more than <span class="tex-span">2</span>. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of balls Limak has.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the size of the <span class="tex-span"><i>i</i></span>-th ball.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if Limak can choose three balls of distinct sizes, such that any two of them differ by no more than <span class="tex-span">2</span>. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
4
18 55 16 17

```




```input2
6
40 41 43 44 44 44

```




```input3
8
5 972 3 4 1 4 970 971

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample, there are <span class="tex-span">4</span> balls and Limak is able to choose three of them to satisfy the rules. He must must choose balls with sizes <span class="tex-span">18</span>, <span class="tex-span">16</span> and <span class="tex-span">17</span>.</p><p>In the second sample, there is no way to give gifts to three friends without breaking the rules.</p><p>In the third sample, there is even more than one way to choose balls:</p><ol> <li> Choose balls with sizes <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span>. </li><li> Choose balls with sizes <span class="tex-span">972</span>, <span class="tex-span">970</span>, <span class="tex-span">971</span>. </li></ol>
