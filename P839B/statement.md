## Description

<div><p>Daenerys Targaryen has an army consisting of <span class="tex-span"><i>k</i></span> groups of soldiers, the <span class="tex-span"><i>i</i></span>-th group contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> soldiers. She wants to bring her army to the other side of the sea to get the Iron Throne. She has recently bought an airplane to carry her army through the sea. The airplane has <span class="tex-span"><i>n</i></span> rows, each of them has <span class="tex-span">8</span> seats. We call two seats neighbor, if they are in the same row and in seats <span class="tex-span">{1, 2}</span>, <span class="tex-span">{3, 4}</span>, <span class="tex-span">{4, 5}</span>, <span class="tex-span">{5, 6}</span> or <span class="tex-span">{7, 8}</span>.</p><center> <img class="tex-graphics" src="file://6lgnJbMC.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">A row in the airplane</span> </center><p>Daenerys Targaryen wants to place her army in the plane so that there are no two soldiers from different groups sitting on neighboring seats.</p><p>Your task is to determine if there is a possible arranging of her army in the airplane such that the condition above is satisfied.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of rows and the number of groups of soldiers, respectively.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of soldiers in the <span class="tex-span"><i>i</i></span>-th group.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 8·<i>n</i></span>.</p></div><div class="output-specification"><p>If we can place the soldiers in the airplane print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of rows and the number of groups of soldiers, respectively.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of soldiers in the <span class="tex-span"><i>i</i></span>-th group.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 8·<i>n</i></span>.</p>

## Output

<p>If we can place the soldiers in the airplane print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p>





```input1
2 2
5 8

```




```input2
1 2
7 1

```




```input3
1 2
4 4

```




```input4
1 4
2 2 1 2

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




```output4
YES

```



## Note

<p>In the first sample, Daenerys can place the soldiers like in the figure below:</p><center> <img class="tex-graphics" src="file://brRBoE6z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, there is no way to place the soldiers in the plane since the second group soldier will always have a seat neighboring to someone from the first group.</p><p>In the third example Daenerys can place the first group on seats <span class="tex-span">(1, 2, 7, 8)</span>, and the second group an all the remaining seats.</p><p>In the fourth example she can place the first two groups on seats <span class="tex-span">(1, 2)</span> and <span class="tex-span">(7, 8)</span>, the third group on seats <span class="tex-span">(3)</span>, and the fourth group on seats <span class="tex-span">(5, 6)</span>.</p>
