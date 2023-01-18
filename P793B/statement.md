## Description

<div><p>Woken up by the alarm clock Igor the financial analyst hurried up to the work. He ate his breakfast and sat in his car. Sadly, when he opened his GPS navigator, he found that some of the roads in Bankopolis, the city where he lives, are closed due to road works. Moreover, Igor has some problems with the steering wheel, so he can make <span class="tex-font-style-bf">no more than two turns</span> on his way to his office in bank.</p><p>Bankopolis looks like a grid of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Igor should find a way from his home to the bank that has no more than two turns and doesn't contain cells with road works, or determine that it is impossible and he should work from home. A turn is a change in movement direction. Igor's car can only move to the left, to the right, upwards and downwards. Initially Igor can choose any direction. Igor is still sleepy, so you should help him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in the grid.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters denoting the corresponding row of the grid. The following characters can occur: </p><ul> <li> "<span class="tex-font-style-tt">.</span>" — an empty cell; </li><li> "<span class="tex-font-style-tt">*</span>" — a cell with road works; </li><li> "<span class="tex-font-style-tt">S</span>" — the cell where Igor's home is located; </li><li> "<span class="tex-font-style-tt">T</span>" — the cell where Igor's office is located. </li></ul><p>It is guaranteed that "<span class="tex-font-style-tt">S</span>" and "<span class="tex-font-style-tt">T</span>" appear exactly once each.</p></div><div class="output-specification"><p>In the only line print "<span class="tex-font-style-tt">YES</span>" if there is a path between Igor's home and Igor's office with no more than two turns, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in the grid.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters denoting the corresponding row of the grid. The following characters can occur: </p><ul> <li> "<span class="tex-font-style-tt">.</span>" — an empty cell; </li><li> "<span class="tex-font-style-tt">*</span>" — a cell with road works; </li><li> "<span class="tex-font-style-tt">S</span>" — the cell where Igor's home is located; </li><li> "<span class="tex-font-style-tt">T</span>" — the cell where Igor's office is located. </li></ul><p>It is guaranteed that "<span class="tex-font-style-tt">S</span>" and "<span class="tex-font-style-tt">T</span>" appear exactly once each.</p>

## Output

<p>In the only line print "<span class="tex-font-style-tt">YES</span>" if there is a path between Igor's home and Igor's office with no more than two turns, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
5 5
..S..
****.
T....
****.
.....

```




```input2
5 5
S....
****.
.....
.****
..T..

```




```output1
YES
```




```output2
NO
```



## Note

<p>The first sample is shown on the following picture:</p><center> <img class="tex-graphics" src="file://WPLxrxq3.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>In the second sample it is impossible to reach Igor's office using less that <span class="tex-span">4</span> turns, thus there exists no path using no more than <span class="tex-span">2</span> turns. The path using exactly <span class="tex-span">4</span> turns is shown on this picture:</p><center> <img class="tex-graphics" src="file://lIvjDzo3.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center>
