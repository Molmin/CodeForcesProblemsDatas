## Description

<div><p>Hiking club "Up the hill" just returned from a walk. Now they are trying to remember which hills they've just walked through.</p><p>It is known that there were <span class="tex-span"><i>N</i></span> stops, all on different integer heights between <span class="tex-span">1</span> and <span class="tex-span"><i>N</i></span> kilometers (inclusive) above the sea level. On the first day they've traveled from the first stop to the second stop, on the second day they've traveled from the second to the third and so on, and on the last day they've traveled from the stop <span class="tex-span"><i>N</i> - 1</span> to the stop <span class="tex-span"><i>N</i></span> and successfully finished their expedition.</p><p>They are trying to find out which heights were their stops located at. They have an entry in a travel journal specifying how many days did they travel up the hill, and how many days did they walk down the hill.</p><p>Help them by suggesting some possible stop heights satisfying numbers from the travel journal.</p></div><div class="input-specification"><p>In the first line there is an integer non-negative number <span class="tex-span"><i>A</i></span> denoting the number of days of climbing up the hill. Second line contains an integer non-negative number <span class="tex-span"><i>B</i></span>&nbsp;— the number of days of walking down the hill (<span class="tex-span"><i>A</i> + <i>B</i> + 1 = <i>N</i></span>, <span class="tex-span">1 ≤ <i>N</i> ≤ 100 000</span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>N</i></span> space-separated distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> inclusive, denoting possible heights of the stops in order of visiting.</p></div>

## Input

<p>In the first line there is an integer non-negative number <span class="tex-span"><i>A</i></span> denoting the number of days of climbing up the hill. Second line contains an integer non-negative number <span class="tex-span"><i>B</i></span>&nbsp;— the number of days of walking down the hill (<span class="tex-span"><i>A</i> + <i>B</i> + 1 = <i>N</i></span>, <span class="tex-span">1 ≤ <i>N</i> ≤ 100 000</span>).</p>

## Output

<p>Output <span class="tex-span"><i>N</i></span> space-separated distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> inclusive, denoting possible heights of the stops in order of visiting.</p>





```input1
0
1

```




```input2
2
1
```




```output1
2 1 

```




```output2
1 3 4 2
```


