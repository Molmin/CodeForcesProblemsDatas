## Description

<div><p>Little boy Igor wants to become a traveller. At first, he decided to visit all the cities of his motherland&nbsp;— Uzhlyandia.</p><p>It is widely known that Uzhlyandia has <span class="tex-span"><i>n</i></span> cities connected with <span class="tex-span"><i>m</i></span> bidirectional roads. Also, there are no two roads in the country that connect the same pair of cities, but roads starting and ending in the same city can exist. Igor wants to plan his journey beforehand. Boy thinks a path is <span class="tex-font-style-it">good</span> if the path goes over <span class="tex-span"><i>m</i> - 2</span> roads twice, and over the other <span class="tex-span">2</span> exactly once. The good path can start and finish in any city of Uzhlyandia.</p><p>Now he wants to know how many different good paths are in Uzhlyandia. Two paths are considered different if the sets of roads the paths goes over exactly once differ. Help Igor&nbsp;— calculate the number of good paths.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>&nbsp;— the number of cities and roads in Uzhlyandia, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) that mean that there is road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>It is guaranteed that no road will be given in the input twice. That also means that for every city there is no more than one road that connects the city to itself.</p></div><div class="output-specification"><p>Print out the only integer&nbsp;— the number of good paths in Uzhlyandia.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>&nbsp;— the number of cities and roads in Uzhlyandia, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) that mean that there is road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>It is guaranteed that no road will be given in the input twice. That also means that for every city there is no more than one road that connects the city to itself.</p>

## Output

<p>Print out the only integer&nbsp;— the number of good paths in Uzhlyandia.</p>





```input1
5 4
1 2
1 3
1 4
1 5

```




```input2
5 3
1 2
2 3
4 5

```




```input3
2 2
1 1
1 2

```




```output1
6
```




```output2
0
```




```output3
1
```



## Note

<p>In first sample test case the good paths are: </p><ul> <li> <span class="tex-span">2 → 1 → 3 → 1 → 4 → 1 → 5</span>, </li><li> <span class="tex-span">2 → 1 → 3 → 1 → 5 → 1 → 4</span>, </li><li> <span class="tex-span">2 → 1 → 4 → 1 → 5 → 1 → 3</span>, </li><li> <span class="tex-span">3 → 1 → 2 → 1 → 4 → 1 → 5</span>, </li><li> <span class="tex-span">3 → 1 → 2 → 1 → 5 → 1 → 4</span>, </li><li> <span class="tex-span">4 → 1 → 2 → 1 → 3 → 1 → 5</span>. </li></ul><p>There are good paths that are same with displayed above, because the sets of roads they pass over once are same: </p><ul> <li> <span class="tex-span">2 → 1 → 4 → 1 → 3 → 1 → 5</span>, </li><li> <span class="tex-span">2 → 1 → 5 → 1 → 3 → 1 → 4</span>, </li><li> <span class="tex-span">2 → 1 → 5 → 1 → 4 → 1 → 3</span>, </li><li> <span class="tex-span">3 → 1 → 4 → 1 → 2 → 1 → 5</span>, </li><li> <span class="tex-span">3 → 1 → 5 → 1 → 2 → 1 → 4</span>, </li><li> <span class="tex-span">4 → 1 → 3 → 1 → 2 → 1 → 5</span>, </li><li> and all the paths in the other direction. </li></ul><p>Thus, the answer is <span class="tex-span">6</span>.</p><p>In the second test case, Igor simply can not walk by all the roads.</p><p>In the third case, Igor walks once over every road.</p>
