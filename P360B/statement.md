## Description

<div><p>Levko has an array that consists of integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span>. But he doesn’t like this array at all.</p><p>Levko thinks that the beauty of the array <span class="tex-span"><i>a</i></span> directly depends on value <span class="tex-span"><i>c</i>(<i>a</i>)</span>, which can be calculated by the formula: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://NudGdmwz.png" style="max-width: 100.0%;max-height: 100.0%;"></center> The less value <span class="tex-span"><i>c</i>(<i>a</i>)</span> is, the more beautiful the array is.<p>It’s time to change the world and Levko is going to change his array for the better. To be exact, Levko wants to change the values of at most <span class="tex-span"><i>k</i></span> array elements (it is allowed to replace the values by any integers). Of course, the changes should make the array as beautiful as possible.</p><p>Help Levko and calculate what minimum number <span class="tex-span"><i>c</i>(<i>a</i>)</span> he can reach.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2000</span>). The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>A single number — the minimum value of <span class="tex-span"><i>c</i>(<i>a</i>)</span> Levko can get.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2000</span>). The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>A single number — the minimum value of <span class="tex-span"><i>c</i>(<i>a</i>)</span> Levko can get.</p>





```input1
5 2
4 7 4 7 4

```




```input2
3 1
-100 0 100

```




```input3
6 3
1 2 3 7 8 9

```




```output1
0

```




```output2
100

```




```output3
1

```



## Note

<p>In the first sample Levko can change the second and fourth elements and get array: <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>.</p><p>In the third sample he can get array: <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>, <span class="tex-span">6</span>.</p>
