## Description

<div><p>Arkady decides to observe a river for <span class="tex-span"><i>n</i></span> consecutive days. The river's water level on each day is equal to some real value.</p><p>Arkady goes to the riverside each day and makes a mark on the side of the channel at the height of the water level, but if it coincides with a mark made before, no new mark is created. The water does not wash the marks away. Arkady writes down the number of marks strictly above the water level each day, on the <span class="tex-span"><i>i</i></span>-th day this value is equal to <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Define <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> as the number of marks strictly under the water level on the <span class="tex-span"><i>i</i></span>-th day. You are to find out the minimum possible sum of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> over all days. There are no marks on the channel before the first day.</p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>)&nbsp;— the number of marks strictly above the water on each day.</p></div><div class="output-specification"><p>Output one single integer&nbsp;— the minimum possible sum of the number of marks strictly below the water level among all days.</p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>)&nbsp;— the number of marks strictly above the water on each day.</p>

## Output

<p>Output one single integer&nbsp;— the minimum possible sum of the number of marks strictly below the water level among all days.</p>





```input1
6
0 1 0 3 0 2

```




```input2
5
0 1 2 1 2

```




```input3
5
0 1 1 2 2

```




```output1
6

```




```output2
1

```




```output3
0

```



## Note

<p>In the first example, the following figure shows an optimal case.</p><center> <img class="tex-graphics" src="file://eQHRZEtt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that on day <span class="tex-span">3</span>, a new mark should be created because if not, there cannot be <span class="tex-span">3</span> marks above water on day <span class="tex-span">4</span>. The total number of marks underwater is <span class="tex-span">0 + 0 + 2 + 0 + 3 + 1 = 6</span>.</p><p>In the second example, the following figure shows an optimal case.</p><center> <img class="tex-graphics" src="file://cn1lNiv4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
