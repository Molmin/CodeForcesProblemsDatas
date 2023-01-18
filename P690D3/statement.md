## Description

<div><p>So many wall designs to choose from! Even modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>, it's an enormous number. Given that recently Heidi acquired an unlimited supply of bricks, her choices are endless! She really needs to do something to narrow them down.</p><p>Heidi is quick to come up with criteria for a <span class="tex-font-style-it">useful</span> wall:</p><ul> <li> In a useful wall, at least one segment is wider than <span class="tex-span"><i>W</i></span> bricks. This should give the zombies something to hit their heads against. Or, </li><li> in a useful wall, at least one column is higher than <span class="tex-span"><i>H</i></span> bricks. This provides a lookout from which zombies can be spotted at a distance. </li></ul><p>This should rule out a fair amount of possibilities, right? Help Heidi compute the number of <span class="tex-font-style-it">useless</span> walls that do not confirm to either of these criteria. In other words, a wall is useless if every segment has width at most <span class="tex-span"><i>W</i></span> and height at most <span class="tex-span"><i>H</i></span>.</p><p>Parameter <span class="tex-span"><i>C</i></span>, the total width of the wall, has the same meaning as in the easy version. However, note that the number of bricks is now unlimited.</p><p>Output the number of useless walls modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p></div><div class="input-specification"><p>The first and the only line of the input contains three space-separated integers <span class="tex-span"><i>C</i></span>, <span class="tex-span"><i>W</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>W</i>, <i>H</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Output the number of different walls, modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>, which are useless according to Heidi's criteria.</p></div>

## Input

<p>The first and the only line of the input contains three space-separated integers <span class="tex-span"><i>C</i></span>, <span class="tex-span"><i>W</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>W</i>, <i>H</i> ≤ 100</span>).</p>

## Output

<p>Output the number of different walls, modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>, which are useless according to Heidi's criteria.</p>





```input1
1 1 1

```




```input2
1 2 2

```




```input3
1 2 3

```




```input4
3 2 2

```




```input5
5 4 9

```




```input6
40 37 65

```




```output1
2

```




```output2
3

```




```output3
4

```




```output4
19

```




```output5
40951

```




```output6
933869

```



## Note

<p>If there is no brick in any of the columns, the structure is considered as a useless wall.</p>
